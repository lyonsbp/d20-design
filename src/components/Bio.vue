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
        <v-subheader
                v-if="item.header"
                :key="item.header"
        >
           Description
        </v-subheader>
            <v-text-field
                    v-model="gender"
                    label="Character Name"
                    required
            ></v-text-field>

        <v-text-field
                v-model="playerName"
                label="Player Name"
                required
        ></v-text-field>
        <v-text-field
                v-model="playerName"
                label="Player Name"
                required
        ></v-text-field>
    </v-form>
</template>

<script>
    import VTextField from "vuetify/src/components/VTextField/VTextField";
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
      },
      components: {VTextField}
    }
</script>

<style scoped>
    input {
        width: 25%;
        border: 2px solid;
    }
</style>