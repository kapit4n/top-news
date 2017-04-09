<template>
  <div id="root">
    <header-component></header-component>
    <main>
      <news-list></news-list>
    </main>
    <footer-component></footer-component>
  </div>
</template>

<script>
import Header from './Header.vue';
import Title from './Title.vue';
import Techs from './techs/Techs.vue';
import newsList from './components/news/newsList.vue';
import Footer from './Footer.vue';

export default {
  name: 'Main',
  components: {
    'header-component': Header,
    'title-component': Title,
    'techs': Techs,
    'footer-component': Footer,
    'news-list': newsList
  }
};
</script>
