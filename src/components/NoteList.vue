<template>
  <ul>
    <note-list-item
      v-for="note in notes"
      :key="note.id"
      :note="note"
      class="
        p-3
        my-4
        border-2 border-white border-gray-
        shadow-xl
        rounded-md
        cursor-pointer
      "
    />
  </ul>
</template>

<script>
import { computed } from "vue";
import { useStore } from "vuex";

import NoteListItem from "./NoteListItem.vue";

export default {
  name: "NodeList",
  components: { NoteListItem },
  setup() {
    const store = useStore();

    // Podemos declararlo directamente desde el retorno ya que realmente nadie más va a utilizar la variable notes
    // const notes = computed(() => store.state.notes);

    return {
      notes: computed(() => store.state.notes),
    };
  },
};
</script>
