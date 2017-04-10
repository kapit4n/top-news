<template>
  <div>
  	 <div class="techs">
      <News v-for="news in newsList" :newsData="news"></News>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import VueResource from 'vue-resource';
Vue.use(VueResource);
import News from './news.vue';
export default {
  name: 'newsList',
  data() {
    return {
      newsList: []
    };
  },
  created() {
    return this.$http
      .get('http://localhost:9000/v1/news'
     )
      .then(response => response.json())
      .then(response => {
        this.newsList = response;
      });
  },
  components: {
    News
  }
};
</script>
