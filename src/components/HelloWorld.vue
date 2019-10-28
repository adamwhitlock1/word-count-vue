<template>
  <div class="font-sans p-4">
    <h1>Enter in some words and get stats.</h1>
    <textarea
      v-model="words"
      class="p-2 border-solid border-2 border-orange-500"
      cols="80"
      rows="20"
    ></textarea>
    <p>Words: {{wordTotal}}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      words: "get started"
    };
  },
  computed: {
    wordTotal() {
      let wordArray = this.words.split(" ");
      return wordArray.length;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
</style>
