<template>
  <section id="SignIn">
    <br>
    <div class="row">
      <div class="col-md-6 offset-md-3">
        <div class="card">
          <div class="card-body">
            <h2 class="card-title text-center">Sign In</h2>
            <form action="#" @submit.prevent="submitSignin">
              <div class="form-group">
                <label for="email" class="sr-only">Email address</label>
                <input type="email" class="form-control form-control-lg" id="email" aria-describedby="emailHelp"
                       placeholder="Enter email" required v-model="formData.email">
                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.
                </small>
              </div>
              <div class="form-group">
                <label for="password" class="sr-only">Password</label>
                <input type="password" class="form-control form-control-lg" id="password" placeholder="Password"
                       required v-model="formData.password">
              </div>
              <router-link to="/sign_up" class="float-right">Sign Up</router-link>
              <button type="submit" class="btn btn-primary btn-lg">Submit</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        formData: {}
      }
    },
    methods: {
      submitSignin() {

      }
    }
  }
</script>

<style scoped>

</style>
