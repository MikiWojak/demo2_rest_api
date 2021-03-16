<template>
  <div id="app">
  </div>
</template>

<script>
import axios from 'axios'

export default {
  data: function() {
    return {
      info: null
    }
  },

  mounted() {
    this.loadInfo();
  },

  methods: {
    loadInfo: function() {
      axios.get('http://localhost:8000/api/user')
      .then((response) => {
        this.info = response;
      })
      .catch(function(error) {
        console.log(error);
      });
    }
  }
}
</script>
