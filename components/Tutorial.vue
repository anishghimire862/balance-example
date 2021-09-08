<!-- Please remove this file from your project -->
<template>
  <div class="relative flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8 items-center text-center">
      <h2 class="text-2xl pb-12 font-semibold">
        {{ server }}
      </h2>
      <iframe :src="src" width="480" height="480" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      server: process.env.SERVER,
      src: process.env.SOURCE,
    };
  },
}
</script>
