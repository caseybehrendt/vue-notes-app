<script>
import NoteSelectors from "./NoteSelectors";
import NoteEditor from "./NoteEditor";

export default {
  components: {
    NoteSelectors,
    NoteEditor,
  },
};
</script>

<template>
  <div class="note-container">
    <NoteSelectors />
    <NoteEditor />
  </div>
</template>
