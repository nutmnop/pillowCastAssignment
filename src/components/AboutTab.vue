<template>
  <div>
    <h3 class="mt-5">About You</h3>
    <b-container fluid class="mt-3">
    <b-row >
      <b-col  class="mt-3 text-left">
        <div class="mt-3 inputBox">
          <div class="ml-2 mr-2">
          <b-form-group>
            <b-container>
              <b-row>
                <b-col><label for="input-1">Display Name</label></b-col>
                <b-col><b-form-text class="text-right">15 characters</b-form-text></b-col>
               </b-row>
            </b-container>
            <b-form-input id="name" v-model="aboutData[0]['name']" v-on:keyup="emitToParent" trim></b-form-input>
          </b-form-group>
          </div>
        </div>
      </b-col>
      <b-col  class="mt-3 ml-2 text-left" >
        <div class="mt-3 inputBox">
          <div class="ml-2 mr-2">
          <b-form-group>
            <b-container>
              <b-row>
                <b-col><label for="tagline">Tagline</label></b-col>
                <b-col><b-form-text class="text-right">15 characters</b-form-text></b-col>
               </b-row>
            </b-container>
            <b-form-input id="tagline" v-model="aboutData[0]['tagline']" trim v-on:keyup="emitToParent"></b-form-input>
          </b-form-group>
          </div>
        </div>
      </b-col>
    </b-row>
      <b-row >
      <b-col class="mt-3 text-left">
        
          <div class="mt-3 inputBox">
          <div class="ml-2 mr-2">
          <b-form-group>
            <b-col><label for="sexual">Sexual</label></b-col>
            <b-form-select id="sexual" trim>
              <option value="M">Male</option>
              <option value="F">Female</option>
              <option value="N">No Gender</option>
            </b-form-select>
          </b-form-group>
          </div>
        </div>
        
      </b-col>
      <b-col class="mt-3 ml-2 text-left" >
       
          <div class="mt-3 inputBox">
          <div class="ml-2 mr-2">
          <b-form-group>
            <b-col><label for="bday">Birthday</label></b-col>
            <b-form-input id="bday"  type="date"></b-form-input>
          </b-form-group>
          </div>
        </div>
        
      </b-col>
    </b-row>
  </b-container>
  </div>  
</template>

<script>

export default {
  name: 'aboutTab',
  data(){
    return{aboutData:[
      {name:'',
      tagline:''}]
    }
  },
   methods: {
    emitToParent (event) {
      this.$emit('childToParent', this.aboutData)
    }
  }
}
</script>


<style scoped>
  .inputBox{
    background-color:#1C2733; 
    width: 100%;
  }
  #name , #tagline, #sexual, #bday{
    background: transparent;
    border: hidden;
    color:white;
    
  }
  option {
    background-color: #1C2733;
    border:hidden;
  }
 
</style>
