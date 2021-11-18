<template>
  <main class="dev | container | p-3 my-3 mx-auto | flex">
    <!--Left side -->
    <section class="dev | p-3 mr-3">
      <!-- Search Notes -->
      <p>Search Notes</p>

      <!-- Note List -->
      <p>Note list</p>
    </section>

    <!-- Right Side -->
    <section class="dev | p-3 | flex-grow">
      <!-- Active note -->
      <p>Active Note</p>
    </section>
  </main>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
.dev {
  border: 1px solid red;
}
</style>
