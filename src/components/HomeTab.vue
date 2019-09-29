<template>
  <div v-if="countData == 0"  align="center">
    <div  class="mt-5">
      <img src="https://icon-library.net/images/found-icon/found-icon-20.jpg">
    </div>
    <h4 class="mt-3" >no upload cast</h4>
    <p class="mt-3">There is no one who loves pain itself, who seks after it and wants to have it, simply because it pain...</p>
    <b-button class="uploadButton" v-on:click="countData+=1">Upload Cast</b-button>
  </div>
  <div v-else>
    <h3 class="mt-5">Your Upload</h3>
    <div class="mt-3">
      <b-container class="bv-example-row">
        <b-row id="card1">
          <b-col cols="4">
            <b-card>
               <b-card overlay class="video" img-src="https://pi.tedcdn.com/r/talkstar-assets.s3.amazonaws.com/production/playlists/playlist_399/podcast_lover_1200x627.jpg?quality=89&w=800">
                 <b-button class="uploadButton mt-3" >Category name</b-button>
               </b-card>
              <b-card-title>
                example text.
              </b-card-title>
              <b-card-text id="creatorName" class="mb-0">
                creator name
              </b-card-text>
              <b-card-text id="srcStat">
                xx minutes ago  1,220  30,000
              </b-card-text>
            </b-card>
          </b-col>
          <b-col cols="4">2 of 3</b-col>
          <b-col cols="4">3 of 3</b-col>
          <b-col cols="4">{{message}}</b-col>
        </b-row>
      </b-container>
      <b-button class="uploadButton" v-on:click="addCard">Upload Cast</b-button>
    </div>
    <b-button class="uploadButton mt-3" v-on:click="countData-=1">Delete Cast</b-button>
  </div>
</template>

<script>
export default {
  name: 'mainTab',
  data:function(){
    return{
      countData:0
    }
  }
}
new Vue({
  el:"#card1",
  data:{
      message:"hi"
  },
  nethods:{
    getMessage:function () {
      return this.message
    }
  }
});
</script>


<style scoped>
 .uploadButton{
   background-image: linear-gradient(to right, #E7C830, #E7B310);
   border-radius: 40px;
 }
 .card{
   background-color: #1C2733;
 }
 #creatorName{
   color: rgb(201, 200, 199);
 }
 #srcStat{
   font-size:80%;
   color: rgb(201, 200, 199);
 }
 
</style>
