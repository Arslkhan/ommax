<template>
  <div class="home">
    <Banner></Banner>
    <Partners></Partners>
    <CompanyProjects></CompanyProjects>
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue';
import Partners from '@/components/Partners.vue';
import CompanyProjects from '@/components/CompanyProjects.vue';
// @ is an alias to /src

export default {
  name: "HomeView",
  components: {
    Banner,
    Partners,
    CompanyProjects
},
};
</script>
