<template>
  <div class="home">
    <Banner></Banner>
    <Partners></Partners>
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue';
import Partners from '@/components/Partners.vue';
// @ is an alias to /src

export default {
  name: "HomeView",
  components: {
    Banner,
    Partners
},
};
</script>
