<template>
  <ul>
    <learning-resource
      v-for="res in storedRecouces"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from './component/leaning-resource/LearningResource.vue';

export default {
  components: {
    LearningResource,
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
