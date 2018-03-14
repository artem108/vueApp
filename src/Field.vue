<template>
  <div>
  <h3>{{ msg }}</h3>
    <input type="text" :value="msg" @input="changeMess"></input>
    <p>{{ mess }}</p>
    {{ test }}
  </div>
</template>

  <script>
      export default {
        props: ['msg', 'test'],
        data() {
          return {
          mess: ''
          }
        },
        methods: {
          changeMess(event) {
            this.mess = event.target.value
            this.$emit('messChange', this.mess)
          }
        }
      }
  </script>
