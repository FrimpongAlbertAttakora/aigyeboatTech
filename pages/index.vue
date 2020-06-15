<template>
  <v-app id="inspire">
    <v-app-bar
      color="#2d98da"
      dark
      shrink-on-scroll
      prominent
      fade-img-on-scroll
      app
    >
      <template v-slot:img="{ props }">
        <v-img v-bind="props"></v-img>
      </template>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-toolbar-title>aigyeboatTechnology</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
      <template v-slot:extension>
        <v-tabs align-with-title grow>
          <v-tab link to="#">Home</v-tab>
          <v-tab link to="#service">Services</v-tab>
          <v-tab link to="#product">Products</v-tab>
          <v-tab link to="#training">Training</v-tab>
          <v-tab link to="#contact">Contact</v-tab>
        </v-tabs>
      </template>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" temporary fixed>
      <v-list dense>
        <v-list-item link to="#">
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="#service">
          <v-list-item-action>
            <v-icon>mdi-book-open</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Services</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="#product">
          <v-list-item-action>
            <v-icon>mdi-book</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Products</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="#training">
          <v-list-item-action>
            <v-icon>mdi-contacts</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Training</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="#contact">
          <v-list-item-action>
            <v-icon>mdi-contacts</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <template>
      <v-carousel show-arrows-on-hover height="500" cycle>
        <v-carousel-item
          v-for="(item, i) in items"
          :key="i"
          :src="item.src"
        ></v-carousel-item>
      </v-carousel>

      <content>
        <v-container>
          <v-row min-height="500" color="#45aaf2">
            <v-col cols="1"></v-col>
            <v-col cols="10">
              <div>
                <h1>About Us</h1>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Officia, suscipit? Officiis delectus nam eligendi recusandae
                  tempora consequatur incidunt unde atque! Beatae, molestiae
                  consectetur ea fugit modi odio omnis quae et.
                </p>
              </div>
            </v-col>
            <v-col cols="1"></v-col>
          </v-row>
          <v-row>
            <v-row>
              <v-col>
                <v-banner
                  id="service"
                  height="100"
                  color="#45aaf2"
                  elevation="12"
                  class="display-1"
                  tile
                >
                  <p class="mt-4">OUR SERVICES</p>
                </v-banner>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="1"></v-col>
              <v-col col="6">
                <h2>CCTV INSTALLATION</h2>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Fugiat rerum alias voluptate! Blanditiis, voluptate. Officia
                  sunt quaerat illo nulla ea, laborum vel aliquam? Voluptatem
                  nemo architecto inventore, quidem eveniet asperiores.
                </p>
              </v-col>
              <v-col col="4">
                <div>
                  <img
                    class="white--text ml-12 d-block"
                    src="~/assets/cctv.jpg"
                    height="250"
                  />
                </div>
              </v-col>
              <v-col cols="1"></v-col>
            </v-row>
            <v-row>
              <v-col cols="1"></v-col>
              <v-col col="6">
                <h2>SOLAR SYSTEMS INSTALLATION</h2>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Fugiat rerum alias voluptate! Blanditiis, voluptate. Officia
                  sunt quaerat illo nulla ea, laborum vel aliquam? Voluptatem
                  nemo architecto inventore, quidem eveniet asperiores.
                </p>
              </v-col>
              <v-col col="4">
                <div>
                  <img
                    class="white--text ml-12 d-block"
                    src="~/assets/solar.jpg"
                    height="250"
                  />
                </div>
              </v-col>
              <v-col cols="1"></v-col>
            </v-row>
            <v-row>
              <v-col cols="1"></v-col>
              <v-col col="6">
                <h2>CAR ALARM AND SECURITY SYSTEMS</h2>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Fugiat rerum alias voluptate! Blanditiis, voluptate. Officia
                  sunt quaerat illo nulla ea, laborum vel aliquam? Voluptatem
                  nemo architecto inventore, quidem eveniet asperiores.
                </p>
              </v-col>
              <v-col col="4">
                <div>
                  <img
                    class="white--text ml-12 d-block"
                    src="~/assets/cartrack1.jpg"
                    height="250"
                  />
                </div>
              </v-col>
              <v-col cols="1"></v-col>
            </v-row>
          </v-row>
          <v-row>
            <v-row>
              <v-col>
                <v-banner
                  id="product"
                  height="100"
                  color="#4b6584"
                  elevation="12"
                  class="display-1"
                  tile
                >
                  <p class="mt-4">PRODUCTS ON SALE</p>
                </v-banner>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="1"></v-col>
              <v-col col="6">
                <h2>SOLAR SYSTEMS INSTALLATION</h2>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Fugiat rerum alias voluptate! Blanditiis, voluptate. Officia
                  sunt quaerat illo nulla ea, laborum vel aliquam? Voluptatem
                  nemo architecto inventore, quidem eveniet asperiores.
                </p>
              </v-col>
              <v-col col="4">
                <div>
                  <img
                    class="white--text ml-12 d-block"
                    src="~/assets/pic_2a.jpg"
                    height="250"
                  />
                </div>
              </v-col>
              <v-col cols="1"></v-col>
            </v-row>
          </v-row>
          <v-row dense>
            <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
              <v-card>
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px"
                >
                  <v-card-title v-text="card.title"></v-card-title>
                </v-img>
              </v-card>
            </v-col>
          </v-row>
          <v-row>
            <v-row>
              <v-col>
                <v-banner
                  id="training"
                  height="100"
                  color="#778ca3"
                  elevation="12"
                  class="display-1"
                  tile
                >
                  <p class="mt-4">TRAINING</p>
                </v-banner>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="1"></v-col>
              <v-col col="6">
                <h2>CCTV INSTALLATION</h2>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Fugiat rerum alias voluptate! Blanditiis, voluptate. Officia
                  sunt quaerat illo nulla ea, laborum vel aliquam? Voluptatem
                  nemo architecto inventore, quidem eveniet asperiores.
                </p>
              </v-col>
              <v-col col="4">
                <div>
                  <img
                    class="white--text ml-12 d-block"
                    src="~/assets/pic_1a.jpg"
                    height="250"
                  />
                </div>
              </v-col>
              <v-col cols="1"></v-col>
            </v-row>
          </v-row>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
        </v-container>
      </content>

      <v-footer dark padless>
        <v-card
          id="contact"
          flat
          tile
          class="primary lighten-1 white--text text-center"
          width="100%"
        >
          <v-card
            class="mx-auto px-5 mt-7"
            width="80%"
            color="#778ca3"
            height="28rem"
            elevation="3"
          >
            <h1>Contact</h1>

            <v-form
              name="contactus"
              action="/"
              method="post"
              netlify
              netlify-honeypot="bot-field"
            >
              <input type="hidden" name="form-name" value="contactus" />
              <v-text-field
                v-model="name"
                name="name"
                :counter="35"
                :rules="nameRules"
                label="Name"
                required
              ></v-text-field>

              <v-text-field
                v-model="email"
                name="email"
                :rules="emailRules"
                label="E-mail"
                required
              ></v-text-field>

              <v-textarea
                name="message"
                filled
                label="Please enter your message, questions or suggestions here !"
                auto-grow
                value=""
                counter="500"
                clearable
              ></v-textarea>

              <v-btn class="mr-4" color="success" type="submit">
                submit
              </v-btn>
            </v-form>
          </v-card>
          <v-card-text>
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4 white--text"
              icon
            >
              <v-icon size="24px">{{ icon }}</v-icon>
            </v-btn>
          </v-card-text>

          <v-card-text class="white--text pt-0">
            <p class="text-left text-uppercase font-italic">
              E-Mail: info@aigyeboatTechnology.com
            </p>
            <p class="text-left text-uppercase font-italic">
              Mobile Number: **********
            </p>
            <p class="text-left text-uppercase font-italic">
              Location: Ejisu-Kumasi, Near Spiritan University
            </p>
          </v-card-text>

          <v-divider></v-divider>

          <v-card-text class="white--text">
            {{ new Date().getFullYear() }} — <strong>frimpTek Media</strong>
          </v-card-text>
        </v-card>
      </v-footer>
    </template>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    items: [
      {
        src: require('~/assets/pic_1a.jpg')
      },
      {
        src: require('~/assets/pic_2a.jpg')
      },
      {
        src: require('~/assets/pic_3a.jpg')
      },
      {
        src: require('~/assets/pic_4a.jpg')
      },
      {
        src: require('~/assets/pic_5a.jpg')
      }
    ],
    cards: [
      {
        title: 'Training',
        src: require('~/assets/pic_3a.jpg'),
        flex: 6
      },
      {
        title: 'Sanitizer machine',
        src: require('~/assets/pic_1a.jpg'),
        flex: 6
      },
      {
        title: 'Handwash machine',
        src: require('~/assets/pic_2a.jpg'),
        flex: 6
      },
      {
        title: 'Training',
        src: require('~/assets/pic_4a.jpg'),
        flex: 6
      }
    ],
    icons: ['mdi-facebook', 'mdi-twitter', 'mdi-linkedin', 'mdi-instagram']
  }),
  head() {
    return {
      title: 'Ageiboat Technology Home | Technology',
      meta: [
        {
          hid:
            'Core Mathematics, Elective Mathematics, Mathematics, WAEC Core Mathematics, Core Mathematics Sylabus, Elective Mathematics Syllabus',
          name:
            'Core Mathematics, Elective Mathematics, Mathematics, WAEC Core Mathematics, Core Mathematics Sylabus, Elective Mathematics Syllabus',
          content:
            'Core Mathematics, Elective Mathematics, Mathematics, WAEC Core Mathematics, Core Mathematics Sylabus, Elective Mathematics Syllabus'
        }
      ]
    }
  }
}
</script>

<style>
footer {
  width: 100vw;
}
</style>
