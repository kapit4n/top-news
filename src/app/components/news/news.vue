<template>
<div style="width: 250px; display: inline-block;  border-style: dotted;" v-if="newsData.title !== 'noTitle' && newsData.imgUrl !== 'noImage'">
	<div v-if="newsData.imgUrl !== 'noImage'">
  	<img v-bind:src="newsData.imgUrl" style="height: 130px;">
	</div >
  <h3 style="font-size: 20px; font-weight: bold;"> <a v-bind:href="newsData.link" style="color: black;">{{ newsData.title }}</a></h3>
  <p style="height: 100px;">{{ newsData.body }}</p>
</div>
</template>

<script>
export default {
  name: 'News',
  props: ['newsData']
};
</script>
