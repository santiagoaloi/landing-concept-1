<template>
  <div class="mt-28">
    <div class="hero-grid">
      <div>
        <div>
          <h1 class="hero-title">
            The next generation
            <span> virtual classroom</span>
          </h1>
          <p class="hero-subtitle pr-2">
            Enable active learning, collaboration, and engagement in online classes and virtual
            instructor-led training.
          </p>

          <HomeHeroActionButtons />
        </div>

        <HomeHeroReviews />
      </div>

      <HomeHeroImg />
    </div>
  </div>
</template>

<style scoped>
.hero-grid {
  @apply grid md:grid-cols-1 lg:grid-cols-2 gap-1 md:gap-8 xl:gap-0 
}

.hero-title {
  @apply  text-5xl font-bold lg:text-6xl 
  
}

.hero-title-gradient {
  @apply bg-clip-text bg-gradient-to-bl from-[#8788ee] to-[#304c85] text-transparent
}

.hero-subtitle {
  @apply mt-3 text-lg text-gray-800 dark:text-gray-400
}
</style>
