<template>
  <v-app id="inspire">
    <v-content>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-14">
              <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="8">
                      <v-card-text class="mt-5">
                        <h1
                          class="text-center display-2 teal--text text--accent-3"
                        >Sign in to WeFit</h1>
                        <v-form>
                          <v-text-field
                            label="Username"
                            name="username"
                            prepend-icon="person"
                            type="text"
                            color="teal accent-3"
                          />

                          <v-text-field
                            id="password"
                            label="Password"
                            name="password"
                            prepend-icon="lock"
                            type="password"
                            color="teal accent-3"
                          />
                        </v-form>
                      </v-card-text>
                      <div class="text-center mb-10">
                        <v-btn rounded color="teal accent-3" dark to="/home">SIGN IN</v-btn>
                      </div>
                    </v-col>
                    <v-col cols="12" md="4" class="teal accent-3">
                      <v-card-text class="white--text mt-12">
                        <h1 class="text-center display-1">New User?</h1>
                        <h3
                          class="text-center my-4"
                        >Enter your personal details and become healthy with us!</h3>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn rounded outlined dark @click="step++" to="/signup">SIGN UP</v-btn>
                      </div>
                    </v-col>
                  </v-row>
<!--                </v-window-item>-->
<!--                <v-window-item :value="2">-->
<!--                  <v-row class="fill-height">-->
<!--                    <v-col cols="12" md="4" class="teal accent-3">-->
<!--                      <v-card-text class="white&#45;&#45;text mt-12">-->
<!--                        <h1 class="text-center display-1">Welcome Back!</h1>-->
<!--                        <h5-->
<!--                          class="text-center"-->
<!--                        >To Keep connected with us please login with your personnel info</h5>-->
<!--                      </v-card-text>-->
<!--                      <div class="text-center">-->
<!--                        <v-btn rounded outlined dark @click="step&#45;&#45;">Sign in</v-btn>-->
<!--                      </div>-->
<!--                    </v-col>-->

<!--                    <v-col cols="12" md="8">-->
<!--                      <v-card-text class="mt-12">-->
<!--                        <h1 class="text-center display-2 teal&#45;&#45;text text&#45;&#45;accent-3">Create Account</h1>-->
<!--                        <div class="text-center mt-4">-->
<!--                          <v-btn class="mx-2" fab color="black" outlined>-->
<!--                            <v-icon>fab fa-facebook-f</v-icon>-->
<!--                          </v-btn>-->

<!--                          <v-btn class="mx-2" fab color="black" outlined>-->
<!--                            <v-icon>fab fa-google-plus-g</v-icon>-->
<!--                          </v-btn>-->
<!--                          <v-btn class="mx-2" fab color="black" outlined>-->
<!--                            <v-icon>fab fa-linkedin-in</v-icon>-->
<!--                          </v-btn>-->
<!--                        </div>-->
<!--                        <h4 class="text-center mt-4">Ensure your email for registration</h4>-->
<!--                        <v-form>-->
<!--                          <v-text-field-->
<!--                            label="Name"-->
<!--                            name="Name"-->
<!--                            prepend-icon="person"-->
<!--                            type="text"-->
<!--                            color="teal accent-3"-->
<!--                          />-->
<!--                          <v-text-field-->
<!--                            label="Email"-->
<!--                            name="Email"-->
<!--                            prepend-icon="email"-->
<!--                            type="text"-->
<!--                            color="teal accent-3"-->
<!--                          />-->

<!--                          <v-text-field-->
<!--                            id="password"-->
<!--                            label="Password"-->
<!--                            name="password"-->
<!--                            prepend-icon="lock"-->
<!--                            type="password"-->
<!--                            color="teal accent-3"-->
<!--                          />-->
<!--                        </v-form>-->
<!--                      </v-card-text>-->
<!--                      <div class="text-center mt-n5">-->
<!--                        <v-btn rounded color="teal accent-3" dark>SIGN UP</v-btn>-->
<!--                      </div>-->
<!--                    </v-col>-->
<!--                  </v-row>-->
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: "Login",
  data: () => ({
    step: 1
  }),
  props: {
    source: String
  }
};

</script>

<!--<style scoped>-->
<!--.fill-height {-->
<!--  background: url('../assets/logo.png');-->
<!--  background-size: cover;-->
<!--}-->
<!--</style>-->