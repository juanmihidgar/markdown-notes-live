<template>
  <main
    class="
      container
      min-h-1/2
      p-3
      my-3
      mx-auto
      bg-white
      rounded-xl
      shadow-lg
      flex
    "
  >
    <!--Left side -->
    <section class="w-1/4 p-3 mr-3 bg-gray-100">
      <!-- Search Notes -->
      <p>Search Notes</p>

      <!-- Note List -->
      <note-list />
    </section>

    <!-- Right Side -->
    <section class="p-3 | flex-grow">
      <!-- Active note -->
      <active-note />
    </section>
  </main>
</template>

<script>
import NoteList from "@/components/NoteList.vue";
import ActiveNote from "@/components/ActiveNote.vue";

export default {
  name: "App",
  components: {
    NoteList,
    ActiveNote,
  },
};
</script>

<style>
.dev {
  border: 1px solid red;
}
</style>
