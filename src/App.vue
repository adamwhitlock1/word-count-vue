<template>
  <div id="app">
    <HelloWorld :items="[
    {
      text: 'item 1',
      link: 'google.com'
    },
    {
      text: 'item 2',
      link: 'google.com'
    },
    {
      text: 'item 3',
      link: 'google.com'
    },
    {
      text: 'item 4',
      link: 'google.com'
    },
    ]" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>

<style>

</style>
