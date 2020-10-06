<template>
  <v-container>
    <h2>{{ $t("customTitle") }}</h2>
    <p> {{ $t("customDescription") }}
    </p>
    <v-form v-model="valid">
      <v-container>
        <v-row>
          <v-col
              cols="12"
              md="4"
          >
            <v-text-field
                v-model="firstname"
                :rules="nameRules"
                :counter="10"
                label="Time"
                required
            ></v-text-field>
          </v-col>

          <v-col
              cols="12"
              md="4"
          >
            <v-text-field
                v-model="lastname"
                :rules="nameRules"
                :counter="10"
                label="Meters"
                required
            ></v-text-field>
          </v-col>

          <v-col
              cols="12"
              md="4"
          >
            <v-text-field
                v-model="email"
                :rules="emailRules"
                label="Feet"
                required
            ></v-text-field>

          </v-col>
          <v-col
          cols="12"
          md="4">
            <v-btn
                :disabled="!valid"
                color="success"
                class="mr-4"
                @click="validate"
            >
            Validate
            </v-btn>

            <v-btn
                color="error"
                class="mr-4"
                @click="reset"
            >
              Reset Form
            </v-btn>

          </v-col>
        </v-row>
      </v-container>
    </v-form>
  </v-container>
</template>

<script>
export default {
  name: 'custom'
}
</script>
