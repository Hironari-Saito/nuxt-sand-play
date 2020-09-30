<template>
  <div>
    <HeaderPattern1 />
    <div class="container-hero">
      <nuxt-link to="/design">See Design</nuxt-link>
      <nuxt-link to="/script">See Script</nuxt-link>
    </div>
    <div class="container-hero bg-gray-100">
      <button class="animate-spin">Spin</button>
      <button class="animate-ping">Ping</button>
      <button class="animate-pulse">Pulse</button>
      <button class="animate-bounce">Bounce</button>
      <iframe src="http://entreschoolonline.com" frameborder="1"></iframe>
      <iframe
        width="560"
        height="315"
        src="https://www.youtube.com/embed/2OyD8Zg_hH0"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.container-hero {
  @apply h-screen;
  @apply flex items-center justify-center;
}
a {
  @apply p-3;
  @apply border;
  @apply transition duration-300;
  @apply border-current;

  color: $base-color;
  &:hover {
    @apply bg-green-400;
    @apply text-white;
  }
}
</style>
