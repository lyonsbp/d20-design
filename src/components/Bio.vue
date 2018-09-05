<template>
    <v-form v-model="bio">
        <v-text-field
            v-model="playerName"
            label="Player Name"
            required
        ></v-text-field>
        <v-text-field
                v-model="characterName"
                label="Character Name"
                required
        ></v-text-field>
        <v-text-field
            v-model="gender"
            label="Gender"
            required
        ></v-text-field>
        <v-text-field
                v-model="age"
                label="Age"
                required
        ></v-text-field>
        <v-text-field
                v-model="hair"
                label="Hair"
                required
        ></v-text-field>
        <v-text-field
                v-model="height"
                label="Height"
                required
        ></v-text-field>
        <v-text-field
                v-model="build"
                label="Build"
                required
        ></v-text-field>
        <v-text-field
                v-model="eyes"
                label="Eyes"
                required
        ></v-text-field>

        <v-textarea
                outline
                v-model="notableFeatures"
                label="Notable Features"
                required
        ></v-textarea>
    </v-form>
</template>

<script>
    export default {
        name: "Bio",
      data () {
          return {
            playerName:'',
            characterName:'',
            motivation:'',
            obligation:'',
            description: {
              gender:'',
              age:0,
              hair:'',
              height:0,
              build:'',
              eyes:'',
              notableFeatures:''
            }
          }
      }
    }
</script>

<style scoped>
    input {
        width: 25%;
        border: 2px solid;
    }
</style>
