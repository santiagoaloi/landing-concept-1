<template>
  <div
    class="absolute inset-0 text-slate-900/[0.07] [mask-image:linear-gradient(to_bottom_left,white,transparent,transparent)]"
  >
    <svg class="absolute inset-0 h-full w-full" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern
          id="grid-bg"
          height="32"
          patternTransform="translate(0 -1)"
          patternUnits="userSpaceOnUse"
          width="32"
          x="100%"
        >
          <path d="M0 32V.5H32" fill="none" stroke="currentColor"></path>
        </pattern>
      </defs>
      <rect fill="url(#grid-bg)" height="100%" width="100%"></rect>
    </svg>
  </div>
</template>
