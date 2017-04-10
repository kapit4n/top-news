<template>
<div style="width: 250px; display: inline-block;">
  <h1>{{ newsData.title }}</h1>
  <p>{{ newsData.body }}</p>
  <img src="http://static.tvtropes.org/pmwiki/pub/images/vegetavwx2014_928.jpg" width="200">
</div>
</template>

<script>
export default {
  name: 'News',
  props: ['newsData']
};
</script>
