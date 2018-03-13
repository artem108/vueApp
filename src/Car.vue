<template>
  <div>
    <app-input :msg="massage"> </app-input>
  </div>
</template>

<script>
  import Input from './Field.vue'

    export default {
      data() {
        return {
          massage: 'Testg'
        }
      },
      components: {
      'app-input': Input
      }
    }
</script>
