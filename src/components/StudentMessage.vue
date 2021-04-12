<template>
  <div>

    <div v-if="student.name">

      <div class="alert alert-info" v-if="student.present">
        Welcome, {{student.name}}
      </div>

      <div class="alert alert-success" v-else>
        Goodbye, {{student.name}}. see you later!
      </div>

    </div>


  </div>
</template>

<script>
export default {
  name:'StudentMesage',
  props:{
    student: Object
  }


}
</script>

<style scoped>

</style>