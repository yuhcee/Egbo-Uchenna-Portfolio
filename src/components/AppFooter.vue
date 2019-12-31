<template>
  <footer>
    <hr />
    <p>All materials &copy; Uchenna Egbo {{ footerYear() }}</p>
    <div class="social-links">
      <a
        :href="`https://twitter.com/${twitter}`"
        target="_blank"
        name="twitter"
      >
        <icon-twitter width="20" height="20" />
      </a>
      &nbsp;
      <a :href="`https://github.com/${github}`" target="_blank" name="github">
        <icon-github width="20" height="20" />
      </a>
      &nbsp;
      <a :href="`https://codepen.io/${codepen}`" target="_blank" name="codepen">
        <icon-codepen width="20" height="20" />
      </a>
    </div>
  </footer>
</template>

<script>
import IconTwitter from './icons/IconTwitter.vue';
import IconGithub from './icons/IconGithub.vue';
import IconCodepen from './icons/IconCodepen.vue';

export default {
  components: {
    IconTwitter,
    IconGithub,
    IconCodepen
  },
  data() {
    return {
      codepen: 'uchennaegbo',
      github: 'uchennaegbo',
      twitter: 'uchesco_'
    };
  },
  methods: {
    footerYear() {
      const currentYear = new Date().getFullYear();
      return currentYear <= '2019' ? '2019' : `2019 - ${currentYear}`;
    }
  }
};
</script>

<style lang="scss" scoped>
footer {
  width: 100vw;
  padding: 50px 8vw 30px;
  div {
    margin-bottom: 30px;
  }
  hr {
    opacity: 0.1;
    margin-bottom: 30px;
  }
  p {
    opacity: 0.7;
    margin-bottom: 30px;
  }
}
</style>
