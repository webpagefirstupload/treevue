<template>
<div id="app">
  <TreeBrowser 
  :node="root"/>
</div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import TreeBrowser from "./components/TreeBrowser.vue";

export default {
  name: "App",
  data() {
    return {
      root: {
        name: '3000', 
        children: [
          {
            name: '2900',
          },
          {
            name: '2800',
          },
          {
            name: '2700',
          },
          {
            name: '2600',
          },
          {
            name: '2500',
          },
          {
            name: '2400',
          },
          {
            name: '2300',
          },
          {
            name: '2200',
          },
          {
            name: '2100',
          },
          {
            name: '2000',
            children: [
              {
                name: '1900'
              },
              {
                name: '1800',
              },
              {
                name: '1700',
              },
              {
                name: '1600',
              },
              {
                name: '1500',
              },
              {
                name: '1400',
              },
              {
                name: '1300',
              },
              {
                name: '1200',
              },
              {
                name: '1100',
              },
            ]
          },
          {
            name: '1000',
            children: [
              {
                name: '900',
              },
              {
                name: '800',
              },
              {
                name: '700',
              },
              {
                name: '600',
              },
              {
                name: '500',
              },
              {
                name: '400',
              },
              {
                name: '300',
              },
              {
                name: '200',
              },
              {
                name: '100',
              },
            ]
          }
        ]
      }
    }
  },

  components: {
    TreeBrowser
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
