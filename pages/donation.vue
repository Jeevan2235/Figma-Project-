<template>
  <v-container>
    <v-card  class="mt-10" color="#e5e5e5" elevation="0" tile>
      <v-container>
        <v-card-title>Yes, I want donate some money</v-card-title>
        <v-card-text class="font-weight-bold">Amount you want to donate</v-card-text>
        <v-row class="ml-1">
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 5,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 10,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 20,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 50,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 1,00,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 5,00,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 10,00,000"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-radio class="font-weight-black"  label="Rs. 20,00,000"></v-radio>
          </v-col>
        </v-row>
        <v-row class="ml-1">
          <v-col class="mt-3" cols="12" md="1">
            <v-radio class="font-weight-black"  label="Others"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-text-field solo></v-text-field>
          </v-col>
        </v-row>
        <v-card-title>Donation For:</v-card-title>

        <v-row class="ml-1">
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Children’s education"></v-radio>
          </v-col>
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Women Empowerment"></v-radio>
          </v-col>
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Food distribution"></v-radio>
          </v-col>
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Drinking Water"></v-radio>
          </v-col>
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Covid Vaccination"></v-radio>
          </v-col>
          <v-col cols="12" md="4">
            <v-radio class="font-weight-black"  label="Elderly Care"></v-radio>
          </v-col>
        </v-row>
        <v-row class="ml-1">
          <v-col class="mt-3" cols="12" md="1">
            <v-radio class="font-weight-black"  label="Others"></v-radio>
          </v-col>
          <v-col cols="12" md="3">
            <v-text-field solo></v-text-field>
          </v-col>
        </v-row>

        <div>
          <v-card-title>Personal Details:</v-card-title>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">Fullname</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">Email</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">Phone no.</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">PAN no.</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">Country</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">Address</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="2">
              <v-card-text class="font-weight-bold">D.O.B</v-card-text>
            </v-col>
            <v-col cols="12" md="6">
              <v-text-field  solo></v-text-field>
            </v-col>
          </v-row>
          <v-row>
            <v-col cols="12" md="7">
              <v-checkbox class="font-weight-black"
                label="I have read through the website's Privacy Policy & Terms and
              Conditions to make a donation."
              ></v-checkbox>
            </v-col>
          </v-row>
          <v-row justify="center">
            <v-btn
              class="mt-3 mb-10 white--text"
              color="#f94f19"
              rounded
              elevation="0"
              height="2.5em"
              width="9em"
            >
              Donate</v-btn
            >
          </v-row>
        </div>
      </v-container>
    </v-card>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        title: "Get in Touch with us",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
      },
    ],
  }),
};
</script>

<style>
</style>