<template>
<div style="width: 250px;">
  <h1>{{ newsData.title }}</h1>
  <p>{{ newsData.description }}</p>
  <img :src="newsData.banner" width="200">
</div>
</template>

<script>
export default {
  name: 'News',
  data() {
    return {
      newsData: {title: 'News title', description: 'This is the news description', banner: 'https://i.ytimg.com/vi/MlxKE1JaGcQ/maxresdefault.jpg'}
    };
  }
};
</script>
