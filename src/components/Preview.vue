<template>
  <div>
    <p>hi im {{name}} </p>
    <v-text-field
      v-model="text"
    ></v-text-field>
  </div>
</template>

<script>
export default {
    data () {
        return {
            name: 'ashley',
            text: null
        }
    }
}
</script>

<style>

</style>
