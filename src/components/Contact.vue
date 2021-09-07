<template>
  <div class="wave-section">
    <v-container class="d-flex justify-center">
      <v-flex class="text-center col-lg-7 col-md-9 col-sm-12 mt-16">
        <h1
          class="contact-title mt-15 text-center"
          style="text-shadow: 2px 2px 4px #000000;"
        >
          Want to Contact Me?
        </h1>
        <p class="contact-p" style="text-shadow: 2px 2px 4px #000000;">
          Whether you have an idea for a project or just want to chat, feel free
          to send me an email!
        </p>
        <template>
          <v-form
            netlify
            ref="form"
            class="contact-form mb-10 mt-7 p-3 "
            v-model="valid"
            name="contact"
            method="POST"
            data-netlify="true"
          >
            <v-container>
              <v-row>
                <v-col cols="12" md="6">
                  <v-text-field
                    name="name"
                    v-model="name"
                    :rules="nameRules"
                    label="Name"
                    required
                  ></v-text-field>
                </v-col>

                <v-col cols="12" md="6">
                  <v-text-field
                    name="email"
                    v-model="email"
                    :rules="emailRules"
                    label="E-mail"
                    required
                  ></v-text-field>
                </v-col>

                <v-col cols="12" md="12">
                  <v-textarea
                    name="message"
                    v-model="message"
                    outlined
                    :rules="messageRules"
                    label="Message"
                    required
                  ></v-textarea>
                </v-col>
                <v-btn @click="submit" class="submit-btn">
                  submit
                </v-btn>
              </v-row>
            </v-container>
          </v-form>
        </template>

        <div class="pb-10">
          <a
            href="https://www.linkedin.com/in/ali-a-81ab8112a"
            target="_blank"
            class="link-btn"
          >
            <v-btn
              large
              style="background-color: #252835;"
              fab
              small
              depressed="true"
              dark
              v-bind="attrs"
              v-on="on"
              class="mr-5"
            >
              <v-icon x-large color="error">fab fa-linkedin</v-icon>
            </v-btn></a
          >
          <a
            href="https://github.com/lukastars"
            target="_blank"
            class="link-btn"
          >
            <v-btn
              large
              style="background-color: #252835;"
              fab
              small
              depressed="true"
              dark
              v-bind="attrs"
              v-on="on"
              class="mr-5"
            >
              <v-icon x-large color="error">fab fa-github</v-icon>
            </v-btn></a
          >
          <a
            href="mailto:ali.ahmed252715@gmail.com"
            target="_blank"
            class="link-btn"
            ><v-btn
              large
              style="background-color: #252835;"
              fab
              small
              depressed="true"
              dark
              v-bind="attrs"
              v-on="on"
            >
              <v-icon x-large color="error">far fa-envelope</v-icon>
            </v-btn></a
          >
        </div>
      </v-flex>
    </v-container>
  </div>
</template>

<script>
const easings = {
  linear: '',
  easeInQuad: '',
  easeOutQuad: '',
  easeInOutQuad: '',
  easeInCubic: '',
  easeOutCubic: '',
  easeInOutCubic: '',
  easeInQuart: '',
  easeOutQuart: '',
  easeInOutQuart: '',
  easeInQuint: '',
  easeOutQuint: '',
  easeInOutQuint: '',
};
export default {
  data() {
    return {
      type: 'selector',
      selector: ['#projects', '#about', '#home'],
      selected: 'Button',
      duration: 700,
      offset: 30,
      easing: 'easeInOutQuad',
      easings: Object.keys(easings),

      valid: false,
      name: '',
      nameRules: [(v) => !!v || 'Name is required'],
      email: '',
      emailRules: [
        (v) => !!v || 'E-mail is required',
        (v) => /.+@.+/.test(v) || 'E-mail must be valid',
      ],
      message: '',
      messageRules: [(v) => !!v || 'Message is required'],
    };
  },
  computed: {
    target() {
      const value = this[this.type];
      if (!isNaN(value)) return Number(value);
      else return value;
    },
    options() {
      return {
        duration: this.duration,
        offset: this.offset,
        easing: this.easing,
      };
    },
  },
  methods: {
    validate() {
      this.$refs.form.validate();
    },
    submit() {
      if (this.valid) {
        const form = document.querySelector('.contact-form');
        HTMLFormElement.prototype.submit.call(form);
      } else {
        this.validate();
      }
    },
  },
};
</script>

<style>
.contact-title {
  font-size: 48px;
  color: #ffff;
  font-family: 'Tienne', serif;
  font-weight: 700;
}
.contact-p {
  font-size: 20px;
  color: #ffff;
  font-family: 'Tienne', serif;
  font-weight: 400;
}
.contact-section {
  background-color: black;
}

.wave-section {
  background-image: url('../assets/wave.svg');
  background-color: #e877a6;
  background-size: 108%;
}

.contact-form {
  background-color: #f5f5f5;
  color: red !important;
  border-radius: 0.5rem;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 10%), 0 2px 4px -1px rgb(0 0 0 / 6%);
}

.contact-form input {
  color: #252835 !important;
}

.submit-btn {
  margin-left: 12px;
  margin-bottom: 12px;

  background-color: #e877a6 !important;
  color: #252835 !important;
}

@media (max-width: 479px) {
  .contact-title {
    font-size: 32px;
  }
  .contact-p {
    font-size: 16px;
  }
}
</style>
