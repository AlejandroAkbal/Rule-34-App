<template>
  <div
    class="relative flex flex-col items-center justify-center max-w-3xl min-h-screen px-4 mx-auto sm:px-6 lg:px-8"
  >
    <main class="p-5 material-container">
      <img
        src="https://cdn.statically.io/img/raw.githubusercontent.com/h=1024,w=1024,q=90/AlejandroAkbal/brand/main/src/assets/Logo_white.png"
        alt="Akbal logo"
        height="1024"
        width="1024"
        class="w-1/2 h-auto mx-auto rounded-full border-util"
      />

      <a
        href="https://akbal.dev/"
        target="_blank"
        class="block px-3 py-1 mx-auto mt-5 mb-3 rounded-full link w-max bg-darkGray-700 border-util"
      >
        Alejandro Akbal
      </a>

      <small class="block text-center text-gray-200">
        The software engineer that created this app, works whenever he has time
        and will.
      </small>
    </main>

    <footer
      class="absolute inset-x-0 bottom-0 p-2 text-xs text-center text-gray-300"
    >
      v{{ app_version }}
    </footer>
  </div>
</template>

<script>
import { version } from '~/package.json'

export default {
  data() {
    return { app_version: version }
  },

  head() {
    return {
      title: 'About',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Information about the creator.',
        },
      ],
    }
  },
}
</script>
