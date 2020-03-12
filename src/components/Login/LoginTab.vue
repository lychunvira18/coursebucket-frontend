<template>
  <div>
    <v-card class="pa-12 mx-auto" width="800">
      <v-container class="pl-8">
        <v-text-field
          label="Username"
          v-model="username"
          outlined
          class="mx-lg-5 mx-md-5 mt-12"
          color="teal accent-3"
          prepend-icon="mdi-account-circle"
        />
        <v-text-field
          label="Password: "
          :type="showPassword ? 'text' : 'password'"
          class="mx-lg-5 mx-md-5 mt-6 "
          :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
          prepend-icon="mdi-lock"
          id="password"
          @click:append="showPassword = !showPassword"
          required
          v-model="password"
          color="teal accent-3"
          outlined
        />
        <v-checkbox label="Remember me" class="ml-12"></v-checkbox>
        <v-btn class="blue white--text ml-12 mt-6 py-2 mb-12" width="90%"
          >Login</v-btn
        >
      </v-container>
    </v-card>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
