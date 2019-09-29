<template>
<div id="banner">
 
  <b-container fluid class="mt-3 mb-5">
    <b-row >
      <b-col cols="4" class="mt-5 text-right">
        <img src="https://lh3.googleusercontent.com/EqwIgFDYL4BQoWHwEmiut78dbwOpaaF204WFc4INCsq6l8XFch_HR29KhlyDLi63QZm1Rl4R2GfatnrDjzAs_NMMITtmKd8ZJeZApiMOmMRcjPrJYEVM9lrAT0xJneGflEtVAht6a2EiDaRHtKwkVXQxhyHciTG_2rYenEr1NmGjaxECZd1CX07_04Td8LSA3LjM6qnQJF7aERHxEqHFgQlkM3oUaQDV3t6Qo4Cc8OShG8duMfHkv1Dz9_QHwdTQsyfGNPqyHyDqCylEc5OWbGhWU82glyP7RC1MXr4cWRtE33-DPZYqszasBeJgQImgswMKMCUWGZOELv4vQAJstHjT8IMt524KCh5jtvQfwsI6TTSO7e4XNihZYHUrW_ILeBrQ0Ry9Wl0IKvS6bam_eMYKT__4N2CC9AEj4i9wz6tIGJIIEGOCdKRcO6KTZKOdEaDaY0tti3t8Sxts8L3gM5UdZqF9n1eQ0WbTR_XPYhYSNakWjP9g4llFo1fHXPZIqoqh00JqthqUkIXcFeed1cAzr2SGfbAFQYJnIHVa4QaIcSw12_XE16CdEohyugwkaJrVHaXzZQh8rRaiK-6vpcDcHTFnyz12FyoBRkHrDKIGMoU7uJUrW99J-6ZwXVsc3suEWOhUt-Jwdzh09xJf7D3eAxcxkydalclgf64xznRbQdfa6T45_A=w1404-h937-no" id="imgprofile">
      </b-col>
      <b-col cols="8" class="mt-3" >
        <b-row class="mt-5 ml-1 text-left">
          <h2><b> {{name}} (@{{tagline}})</b></h2>
        </b-row>
        <b-row class="mt-2 ml-1 text-left">
          <p>30,000 30,000</p>
        </b-row>
        <b-row class="mt-2 ml-1 text-left">
          <h6> 34 Casts &#9679; 4,500 Followers &#9679; 300 Following</h6>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</div>
</template>

<script>
export default {
  name: 'banner',
  props: {
    name:String,
    tagline:String
  },
  data(){
    return{
      
    }
  }
}
</script>


<style scoped>
  #banner{
    height: 300px;
    background-image: linear-gradient(to bottom, rgba(0,0,0,0.7) 0%,rgba(0,0,0,0.7) 100%),url("https://lh3.googleusercontent.com/EqwIgFDYL4BQoWHwEmiut78dbwOpaaF204WFc4INCsq6l8XFch_HR29KhlyDLi63QZm1Rl4R2GfatnrDjzAs_NMMITtmKd8ZJeZApiMOmMRcjPrJYEVM9lrAT0xJneGflEtVAht6a2EiDaRHtKwkVXQxhyHciTG_2rYenEr1NmGjaxECZd1CX07_04Td8LSA3LjM6qnQJF7aERHxEqHFgQlkM3oUaQDV3t6Qo4Cc8OShG8duMfHkv1Dz9_QHwdTQsyfGNPqyHyDqCylEc5OWbGhWU82glyP7RC1MXr4cWRtE33-DPZYqszasBeJgQImgswMKMCUWGZOELv4vQAJstHjT8IMt524KCh5jtvQfwsI6TTSO7e4XNihZYHUrW_ILeBrQ0Ry9Wl0IKvS6bam_eMYKT__4N2CC9AEj4i9wz6tIGJIIEGOCdKRcO6KTZKOdEaDaY0tti3t8Sxts8L3gM5UdZqF9n1eQ0WbTR_XPYhYSNakWjP9g4llFo1fHXPZIqoqh00JqthqUkIXcFeed1cAzr2SGfbAFQYJnIHVa4QaIcSw12_XE16CdEohyugwkaJrVHaXzZQh8rRaiK-6vpcDcHTFnyz12FyoBRkHrDKIGMoU7uJUrW99J-6ZwXVsc3suEWOhUt-Jwdzh09xJf7D3eAxcxkydalclgf64xznRbQdfa6T45_A=w1404-h937-no");
    background-position: center center;
    background-size: 100% 200%; 
    background-repeat: no-repeat;
  }
 
  #imgprofile{
    width: 40%;
    height: 150px;
    border-radius: 100%;
  }
</style>
