<template>
  <div>
    <v-card height="180" width="900" flat class="ma-12">
      <v-row>
        <v-col xl="4" lg="4" md="4" sm="4" cols="4">
          <v-img
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSM88amYpZVA8Twxi51RyAYacqzRJTPQ-z5GjCyE7665zKSzx-w"
            width="100%"
            height="90%"
          ></v-img>
        </v-col>
        <v-col xl="8" lg="8" md="8" sm="8" cols="8">
          <v-card-title
            ><h3>Web App Review - Semester 3</h3>
            <v-layout justify-end
              >{{ good }}
              <v-btn icon
                ><v-icon class=" mx-2" @click="good += 1">
                  mdi-thumb-up</v-icon
                ></v-btn
              >
              {{ bad }}
              <v-btn icon
                ><v-icon class=" ml-2" @click="bad += 1">
                  mdi-thumb-down</v-icon
                ></v-btn
              >
            </v-layout>
          </v-card-title>
          <v-card-text
            ><h3>Hun Vikran</h3>

            <h3>Professional Procasinator</h3>
          </v-card-text>
          <v-card-action>
            <v-btn text>
              <v-icon class="mr-2">mdi-wechat</v-icon> {{ cmt }} Comment
            </v-btn>
            <v-btn text
              ><v-icon class="mr-2"> mdi-share-variant</v-icon>Share
            </v-btn>
            <v-btn text
              ><v-icon text class="mr-2">mdi-bookmark-outline</v-icon>
              Save</v-btn
            >
          </v-card-action>
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    cmt: 2,
    good: 10,
    bad: 12
  })
};
</script>

<style></style>
