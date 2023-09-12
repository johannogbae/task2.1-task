<template>
    <div>
      <!-- Text Input -->
      <input v-model="text" placeholder="Type something" />
      <p>Text: {{ text }}</p> <br/><br/>
  
      <!-- Checkbox Input -->
      <input type="checkbox" v-model="checked" />
      <label>Checked: {{ checked }}</label> <br/><br/>
  
      <!-- Radio Input -->
      <input type="radio" id="option1" value="Option 1 " v-model="selectedOption" />
      <label for="option1">Option 1 </label>
      <input type="radio" id="option2" value="Option 2 " v-model="selectedOption" />
      <label for="option2">Option 2 </label>
      <p>Selected Option: {{ selectedOption }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        text: '',
        checked: false,
        selectedOption: '',
      };
    },
  };
  </script>
  