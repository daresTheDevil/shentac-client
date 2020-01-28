<template>
  <div>
    <v-carousel :show-arrows="false" cycle>
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        gradient="to top right, rgba(38,50,56,.8), rgba(84,110,122,.4)"
      >
        <v-container fill-height>
          <v-row>
            <v-col cols="auto">
              <h1 class="white--text display-3 font-weight-bold">
                {{ item.title }}
              </h1>
              <a class="white--text headline">{{ item.text }}</a>
            </v-col>
          </v-row>
        </v-container></v-carousel-item
      >
    </v-carousel>
    <!-- <v-img
      src="pistol-sig.jpg"
      height="400"
      gradient="to top right, rgba(100,115,201,.5), rgba(25,32,72,.9)"
    >
      <v-container fill-height>
        <v-row>
          <v-col>
            <h1 class="display-3 white--text font-weight-bold">Safety first</h1>
            <a href="#" class="white--text headline">
              Learn more about our courses
            </a>
          </v-col>
        </v-row>
      </v-container>
    </v-img> -->
    <section class="pt-12 pb-8">
      <v-container>
        <v-row justify="center">
          <v-col cols="auto">
            <h1 class="display-2 text-center">Our Courses</h1>
            <p style="max-width: 60ch;">
              We teach you how to shoot guns and stuff.
            </p>
          </v-col>
        </v-row>
        <v-row>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="basic.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Basic Handgun Skills & Marksmanship
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="advanced.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Advanced Handgun Skills & Marksmanship
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="concealed.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Enhanced Concealed Carry for Mississippi
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section class="py-8">
      <v-container>
        <v-row justify="center">
          <v-col cols="auto">
            <h1 class="display-2 text-center">Security Services</h1>
            <p style="max-width: 60ch;">
              Shenandoah Tactical has 30 years of experience in military and
              federal law enforcement and can provide security surveys, private
              investigative services and private security.
            </p>
          </v-col>
        </v-row>
        <v-row>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="security-survey.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Security Surveys
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="private-eye.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Private Investigative Services
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-card-text>
                <img src="security.svg" width="125" />
              </v-card-text>
              <v-card-text class="py-0">
                <h1 class="headline">
                  Private Security
                </h1>
              </v-card-text>
              <v-card-text>
                The following is placeholder text known as “lorem ipsum,” which
                is scrambled Latin used by designers to mimic real copy.
                Maecenas non leo laoreet, condimentum lorem nec, vulputate
                massa. Mauris egestas at nibh nec finibus.
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="py-8">
      <v-container>
        <v-row justify="center">
          <v-col cols="auto">
            <h1 class="display-2 text-center">We are Shenandoah Tactical</h1>
          </v-col>
        </v-row>
        <v-row>
          <v-col sm="12" md="4">
            <v-card
              :raised="$vuetify.breakpoint.smAndUp"
              :outlined="$vuetify.breakpoint.smAndDown"
            >
              <v-img src="training-opa.jpg" />
              <v-card-text>
                <h1 class="title">
                  Robert Kay
                </h1>
                <p>30 years of experience shooting guns and stuff.</p>
              </v-card-text>
              <v-card-actions>
                <v-spacer />
                <v-btn depressed dark>Learn More</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
export default {
  components: {},
  data: () => ({
    items: [
      {
        src: 'opa-range.jpg',
        title: 'Self Defense',
        text: 'We can put some text here'
      },
      {
        src: 'pistol-sig.jpg',
        title: 'Concealed Carry',
        text: 'Some more text goes here'
      }
    ]
  })
}
</script>
