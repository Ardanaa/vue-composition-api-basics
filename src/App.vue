<template>
  <div class="w-full h-full ">
    <div class="flex justify-center">
      <nav class="flex gap-2">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>

    <div class="mx-auto mt-10">
      <RouterView />
    </div>
  </div>
</template>