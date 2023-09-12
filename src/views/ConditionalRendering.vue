<template>
    <div>
      <h1 v-if="showTitle">Vue is awesome!</h1>
      <h1 v-else>Is Vue awesome?</h1>
      <button @click="toggleTitle">Toggle</button>
      <p v-show="showParagraph">This paragraph is shown with v-show.</p>
      <ul>
        <li v-for="item in items" :key="item.id">{{ item.name }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showTitle: true,
        showParagraph: true,
        items: [
          { id: 1, name: 'Item 1' },
          { id: 2, name: 'Item 2' },
          { id: 3, name: 'Item 3' },
        ],
      };
    },
    methods: {
      toggleTitle() {
        this.showTitle = !this.showTitle;
      },
    },
  };
  </script>
  