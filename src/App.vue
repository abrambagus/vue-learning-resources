<template>
  <the-header title="RememberMe"></the-header>
  <stored-resources :resources="storedRecouces"></stored-resources>
</template>

<script>
import StoredResources from './component/leaning-resource/StoredReasources.vue';
import TheHeader from './component/layouts/TheHeader.vue';

export default {
  components: {
    StoredResources,
    TheHeader,
  },
  data() {
    return {
      storedRecouces: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official documentation.',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to google...',
          link: 'https://google.com',
        },
      ],
    };
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
