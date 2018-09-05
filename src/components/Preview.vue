<template>
  <div>
    <p>hi im {{name}} </p>
    <v-text-field
      v-model="text"
    ></v-text-field>
    <p>value:{{text}}</p>
    <v-btn
      @click="changeText"
    >test
    </v-btn>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'ashley',
      text: null
    }
  },
  methods: {
    changeText () {
      this.text = 'hi bitch'
    }
  }
}
</script>

<style>

</style>
