<template>
  <div> 
    <Banner :name="name" :tagline="tagline"/>
    <b-tabs variant="faded" class="mt-3 newmargin">
      <b-tab title="Home" active><HomeTab/></b-tab>
      <b-tab title="about"><AboutTab v-on:childToParent="onChildClick"/></b-tab>
    </b-tabs>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeTab from '@/components/HomeTab.vue';
import AboutTab from '@/components/AboutTab.vue';
import Banner from '@/components/Banner.vue';
export default {
  name: 'home',
  components: {
    HomeTab,
    AboutTab,
    Banner
  },
  data(){
        return {
      aboutdata:Object,
      name:'',
      tagline:''
    }
  },
  methods: {
    onChildClick (value) {
      this.name=value[0]['name'];
      this.tagline=value[0]['tagline'];
    }
  }
}
</script>

<style scoped>
  .newmargin{
    margin: 0 auto;    
    width: 75%;
  }
</style>
