<template>
  <v-row>
    <v-img src="1.jpg" height="340px" width="1600px">
      <v-row justify="center">
        <h1 class="white--text" style="font-size: 72px; margin-top: 120px">
          Gallery
        </h1>
      </v-row>
    </v-img>

    <v-container>
      <v-row>
        <v-col v-for="n in 12" :key="n" class="d-flex child-flex" cols="3">
          <v-img
            :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
            aspect-ratio="1"
            class="ma-5 grey lighten-2"
          >
            <template v-slot:placeholder>
              <v-row class="fill-height ma-0" align="center" justify="center">
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-col>
      </v-row>
    </v-container>
  </v-row>
</template>