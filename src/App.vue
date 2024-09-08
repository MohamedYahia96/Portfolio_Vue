<template>
  <v-app>
    <!-- nav section  ----------------------->
    <v-app-bar>
      <h1 class="ml-5" style="color: green">
        Portofolio<span style="color: red">.in</span>
      </h1>
      <v-spacer></v-spacer>
      <v-tabs active-class="active-tab" center-active style="font-weight: bold">
        <v-tab href="#home">Home</v-tab>
        <v-tab href="#about">About</v-tab>
        <v-tab href="#porto">Portofolio</v-tab>
        <v-tab href="#blog">Blog</v-tab>
        <v-tab href="#contact">Contact</v-tab>
      </v-tabs>

      <v-btn class="bg-green ml-10 mr-5">Fire me an Email</v-btn>
    </v-app-bar>
    <!-- Main section  ----------------------->
    <v-main>
      <!-- home section -->
      <v-section class="home" id="home">
        <v-row class="align-center px-10" style="height: 690px">
          <v-col cols="6" lg="6" class="pa-6 py-16 font-weight-bold">
            <v-subheader class="text-h2 display-3">
              Visual <span class="text-green"> Design </span> &
              <span style="color: red">Art</span> Director
            </v-subheader>
            <br />
            <br />
            <v-subheader class="">
              Hi , I am Yahia focusing on creating emotional experiennce
            </v-subheader>
            <br />

            <v-btn large elevation="5" class="bg-green mt-9 pb-5 pt-3 px-10">
              Hire Me
            </v-btn>
            <v-btn large elevation="5" class="bg-red mt-9 ml-5 pb-5 pt-3 px-10">
              Contact
            </v-btn>

            <v-row class="mt-16">
              <v-col cols="12">
                <v-chip class="ma-3 px-4 bg-primary">
                  <v-icon size="20">mdi-facebook</v-icon>
                  Facebook
                </v-chip>

                <v-chip class="ma-3 px-4" style="background-color: #01ff56">
                  <v-icon size="20">mdi-whatsapp</v-icon>
                  WhatsApp
                </v-chip>

                <v-chip class="ma-3 px-4 bg-info">
                  <v-icon size="20">mdi-linkedin</v-icon>
                  Linkedin
                </v-chip>

                <v-chip class="ma-3 px-4 bg-dark">
                  <v-icon size="20">mdi-github</v-icon>
                  Githube
                </v-chip>
              </v-col>
            </v-row>
          </v-col>

          <v-col cols="6" lg="6" class="d-flex justify-center">
            <img
              width="70%"
              src="https://www.svgrepo.com/show/192244/man-user.svg"
              alt=""
            />
          </v-col>
        </v-row>
      </v-section>
      <!-- about section -->
      <v-section class="about" id="about">
        <v-container>
          <h1 class="text-center pb-5 pt-10 mt-10">About Me</h1>

          <v-img
            class="pa-10"
            height="400"
            src="https://img.freepik.com/free-vector/office-background-video-conferencing_23-2148656945.jpg"
            alt=""
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
          >
            <v-row justify="center" class="align-center">
              <v-col cols="6" lg="6">
                <v-card class="text-center pa-6 rounded-lg" elevation="6">
                  <v-card-subtitle
                    class="text-h5 font-weight-bold"
                    style="color: green"
                    >About me</v-card-subtitle
                  >
                  <v-card-text class="mt text-h7">
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                    Molestiae sequi omnis officia commodi nesciunt porro,
                    delectus voluptatibus eaque odit veniam et, tempora quia
                    fugiat molestias consectetur! Aspernatur iure praesentium!
                  </v-card-text>

                  <v-btn elevation="6" class="bg-red mt-10 px-10 pb-8 pt-3">
                    Download Resume
                    <v-icon>mdi-download</v-icon>
                  </v-btn>
                </v-card>
              </v-col>

              <v-col cols="6" lg="6">
                <v-card class="pa-6 rounded-lg" elevation="6">
                  <div
                    class="py-1"
                    v-for="(item, index) in proarri"
                    :key="index"
                  >
                    <label>{{ item.title }}</label>
                    <v-progress-linear
                      height="10"
                      :color="item.color"
                      :value="item.value"
                    ></v-progress-linear>
                  </div>
                </v-card>
              </v-col>
            </v-row>
          </v-img>
        </v-container>
      </v-section>
      <!-- education section -->
      <v-section class="education">
        <v-container>
          <h1 class="display-2 text-center">Education</h1>
          <v-row class="py-8">
            <v-col cols="12" lg="6">
              <v-card class="pa-6 rounded-xl" elevation="6">
                <div class="d-flex align-center justify-space-between">
                  <div>
                    <h3>User Experience Designer</h3>
                    <span>March 2024 - Present</span>
                  </div>
                  <div>
                    <a class="text-green"
                      >at Dalian University <v-icon>mdi-link</v-icon></a
                    >
                  </div>
                </div>

                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem
                  obcaecati a perferendis ut quis, distinctio ratione?
                  Distinctio, non eligendi sed laboriosam eum, perferendis
                  reprehenderit unde doloribus saepe eveniet aspernatur
                  repudiandae.
                </v-card-text>
              </v-card>
            </v-col>

            <v-col cols="12" lg="6">
              <v-card class="pa-6 rounded-xl" elevation="6">
                <div class="d-flex align-center justify-space-between">
                  <div>
                    <h3>UI Designer</h3>
                    <span>March 2024 - Present</span>
                  </div>
                  <div>
                    <a class="text-green"
                      >at School University <v-icon>mdi-link</v-icon></a
                    >
                  </div>
                </div>

                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem
                  obcaecati a perferendis ut quis, distinctio ratione?
                  Distinctio, non eligendi sed laboriosam eum, perferendis
                  reprehenderit unde doloribus saepe eveniet aspernatur
                  repudiandae.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-section>
      <!-- Experiance section -->
      <v-section>
        <v-img
          class="pa-10"
          gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
          src="https://designshack.net/wp-content/uploads/Home-office.jpg"
        >
          <v-container>
            <h1 class="text-center">Experience</h1>

            <v-timeline>
              <v-timeline-item
                v-for="(item, index) in experarri"
                :key="index"
                style="color: red"
              >
                <v-card class="rounded-xl">
                  <v-card-title>{{ item.title }}</v-card-title>
                  <v-card-text>
                    <b>{{ item.date }}</b> <br />
                    <b>@ {{ item.institute }}</b> <br />
                    {{ item.description }}
                  </v-card-text>
                </v-card>
              </v-timeline-item>
            </v-timeline>
          </v-container>
        </v-img>
      </v-section>
      <!-- Portofolio section -->
      <v-section class="porto" id="porto">
        <v-container>
          <h1 class="text-center pb-5 mt-5">Portofolio</h1>

          <v-slide-group class="pa-8">
            <v-slide-item v-for="(item, index) in sliarri" :key="index">
              <v-card height="300" width="300" class="mx-2">
                <v-img height="100%" width="100%" :src="item"></v-img>
              </v-card>
            </v-slide-item>
          </v-slide-group>
        </v-container>
      </v-section>
      <!-- contact section -->
      <v-section class="contact" id="contact">
        <v-img
          class="mt-10"
          gradient="to bottom, rgb(166 , 199, 156), rgb(227, 227, 227 /86 %)"
          src="https://img.freepik.com/premium-photo/contact-us-customer-support-hotline-people-connect-call-customer-support-email-address-live-chat-internet-wifi_36325-3415.jpg?w=2000"
        >
          <v-container>
            <h2 class="text-center text-white">
              Always try your Best , and you will find your way . Never give up
              , the best is yet to come Always try your Best , and you will find
              your way . Never give up ,
            </h2>
            <v-divider class="mt-5" color="white" style="border: 2px solid" />

            <v-row>
              <v-col cols="12" lg="6">
                <v-card class="mt-10 bg-transparent text-white">
                  <v-card-title> Drop A Line</v-card-title>

                  <v-form class="justify-center">
                    <v-text-field label="Your Name"></v-text-field>
                    <v-text-field label="Email"></v-text-field>
                    <v-text-field label="Subject"></v-text-field>
                    <v-textarea label="Message"></v-textarea>

                    <v-btn class="bg-green">Send Message</v-btn>
                  </v-form>
                </v-card>
              </v-col>

              <v-col cols="12" lg="3" offset="2">
                <v-card-title> Contact Me</v-card-title>

                <v-subheader class="text-white">
                  4567 Franklin avenue , Arsh cape <br />
                  +382-233-3333 <br />
                  hello@.com
                </v-subheader>

                <v-btn elevation="6" class="bg-red mt-10 px-10 pb-8 pt-3">
                  Download Resume
                  <v-icon>mdi-download</v-icon>
                </v-btn>
              </v-col>
            </v-row>
          </v-container>

          <v-footer class="bg-transparent text-white">
            <v-col cols="12" class="text-center">
              <strong>
                Copyrights @ {{ new Date().getFullYear() }} All rights Reserved
                | This is Made by M.Yahia</strong
              >
            </v-col>
          </v-footer>
        </v-img>
      </v-section>
    </v-main>
  </v-app>
</template>

<script setup>
// import { Nav } from "./components/NavSection.vue";
import { ref } from "vue";

const proarri = ref([
  { title: "HTML", value: 100, color: "light-blue" },
  { title: "CSS", value: 100, color: "deep-orange" },
  { title: "Javascript", value: 70, color: "light-green" },
  { title: "Vuejs", value: 80, color: "blue" },
  { title: "Vuetify", value: 90, color: "black" },
  { title: "PHP", value: 100, color: "red" },
]);

const experarri = ref([
  {
    title: "User Experience Desinger",
    date: "March 2024 - present",
    institute: "Web School",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Auteobcaecati a perferendis ut quis, distinctio ratione",
  },
  {
    title: "UI Desinger",
    date: "March 2024 - present",
    institute: "Web School",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Auteobcaecati a perferendis ut quis, distinctio ratione",
  },
  {
    title: "Graphic Desinger",
    date: "March 2024 - present",
    institute: "Web School",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Auteobcaecati a perferendis ut quis, distinctio ratione",
  },
  {
    title: "Illustration Desinger",
    date: "March 2024 - present",
    institute: "Web School",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Auteobcaecati a perferendis ut quis, distinctio ratione",
  },
]);

const sliarri = ref([
  "data:image/jpeg;base64,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",
  "https://m.media-amazon.com/images/I/71izIFr2ROL._AC_UF894,1000_QL80_.jpg",
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRUGImEc2rk2o44YyDl7WhYtLbzNulHFACNBtrbXvGNAv0abbLavWdnTiskF86KgTch72E&usqp=CAU",
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ-TdG2WfMuUSmaFZUwRYnTv-rI3Yg_IHUqpAPOKFDZsgopjUw0Uet09GpJl-rTsf9l-xY&usqp=CAU",
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSpdSocn9h2kKP3uUi9bQiyw0TT1T6-KE8_i5xHUlAdp_rH8MWjn5BTmZClyR4BRzQF2sY&usqp=CAU",
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSd9mVgsS3SDBMPNAPtRdtBH5ixxhBIznG7MYIVJ98PFZKLeVhxhj6PEazwigWQ0_eIvGQ&usqp=CAU",
]);
</script>

<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
