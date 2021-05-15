<template>
  <nav class="fixed left-0 top-0 bottom-0 h-full">
    <div
      class="
        nav-link
        h-1/3
        flex
        align-middle
        justify-center
        text-center
        bg-white
      "
    >
      <a
        href="#about"
        class="uppercase py-3 px-4 block font-medium text-white bg-blue-500"
        >About</a
      >
    </div>
    <div
      class="
        nav-link
        h-1/3
        flex
        align-middle
        justify-center
        text-center
        bg-white
        text-blue-500
        hover:bg-blue-500
        hover:text-white
      "
    >
      <a href="#projects" class="uppercase py-3 px-4 block">Projects</a>
    </div>
    <div
      class="
        nav-link
        h-1/3
        flex
        align-middle
        justify-center
        text-center
        bg-green-500
        text-white
        hover:bg-white
        hover:text-green-500
      "
    >
      <a href="#skills" class="uppercase py-3 px-4 block">Skills</a>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'TheNavbar',
}
</script>

<style scoped>
.nav-link a {
  font-family: 'Monoton', cursive;
  writing-mode: vertical-lr;
  text-orientation: sideways;
}
</style>
