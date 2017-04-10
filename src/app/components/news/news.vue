<template>
<div style="width: 250px; display: inline-block;" v-if="newsData.title !== 'noTitle'">
  <h3> <a v-bind:href="newsData.link" style="color: black;">{{ newsData.title }}</a></h3>
  <p>{{ newsData.body }}</p>
	<div v-if="newsData.imgUrl !== 'noImage'">
  	<img v-bind:src="newsData.imgUrl" style="max-width: 150px;">
	</div>
</div>
</template>

<script>
export default {
  name: 'News',
  props: ['newsData']
};
</script>
