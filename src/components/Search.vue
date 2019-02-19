<template style="position: relative">
  <section>
    <form class="search-form" v-on:submit.prevent>
      <input type="text" placeholder="What Are You Looking For?" v-model="input" @input="inputChanged" @blur="closeResults">
      <button class="button-unstyled">
        <img src="ic/black/ic_search.png" alt="Search">
      </button>
    </form>

    <div class="search-result-container" v-if="loading">
      <div class="search-result-wrapper">
        <div class="loader"></div>
      </div>
    </div>

    <div class="search-result-container" v-if="showResult">
      <div class="search-result-wrapper">
        <p>
          <span v-if="response">{{response.data.count}}</span>
          <span v-else>0</span>
          Results
        </p>

        <p v-show="response && response.data.count === 0">
          These are not the droids you are looking for...
        </p>

        <ul>
          <li v-for="result in response.data.results" @mousedown="searchElementClicked(result.url)">{{result.name}}, {{result.birth_year}}</li>
        </ul>
      </div>
    </div>

  </section>
</template>

<script>
  import _ from 'lodash';
  import axios from 'axios';

  export default {
    name: 'Search',
    data(){
      return{
        input:"",
        loading: false,
        response:null
      }
    },
    computed:{
      showResult(){
        // Check to see if there are any results in any category.
        if(this.input !== "" && this.response != null){
          return true;
        }
        return false;
      }
    },
    watch:{
      input(){
        if(this.input === ""){
          this.response = null;
        }
      }
    },
    methods:{
      inputChanged: _.debounce(function (){
        // TODO - Multi - category
        if(this.input === ""){
            return;
        }

        this.loading = true;
        axios.get('https://swapi.co/api/people/',{
          params:{
              search: this.input
          }
        })
        .then((response) => {
          this.loading = false;
          this.response = response;
        })
        .catch((response) => {
          console.log("Error Retrieving API query.")
          console.log(response)
          this.loading = false;
        });

      },500),
      closeResults(){
          // TODO - Better Implementation of out of focus clear.
          this.input = "";
      },
      searchElementClicked(url){
        console.log("Will Visit: " + url);
      }
    },
  }
</script>