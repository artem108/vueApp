<template>
  <div>
    <app-input :msg="massage, test" @messChange="massage = $event"> </app-input>
  </div>
</template>

<script>
  import Input from './Field.vue'

    export default {
      data() {
        return {
          massage: 'Test',
          test: 'massage'
        }
      },
      components: {
      'app-input': Input
      }
    }
</script>
