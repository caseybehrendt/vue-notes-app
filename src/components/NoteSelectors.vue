<script>
import NoteSelector from "./NoteSelector";

export default {
  components: {
    NoteSelector,
  },
  data: function () {
    return {
      notes: [
        { id: 1, body: "This is a first note", timestamp: Date.now() },
        { id: 2, body: "This is a second note", timestamp: Date.now() },
        { id: 3, body: "This is a third note", timestamp: Date.now() },
        { id: 4, body: "This is a fourth note", timestamp: Date.now() },
      ],
    };
  },
};
</script>

<template>
  <div class="note-selectors">
    <NoteSelector v-for="note in notes" v-bind:key="note.id" v-bind:note="note" />
  </div>
</template>
