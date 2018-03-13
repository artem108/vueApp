<template>
  <div>
  <h3>{{ msg }}</h3>
    <input type="text" :value="msg" @input=''></input>
    <p>{{ mess }}</p>
  </div>
</template>

  <script>
      export default {
        props: ['msg'],
        data() {
          return {
          mess: ''
          }
        }
      }
  </script>
