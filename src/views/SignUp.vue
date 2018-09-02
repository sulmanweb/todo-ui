<template>
  <section id="SignUp">
    <br>
    <div class="row">
      <div class="col-md-8 offset-md-2">
        <div class="card">
          <div class="card-body">
            <h2 class="card-title text-center">Sign Up</h2>
            <div class="card-text">
              <form action="#" @submit.prevent="submitSignup">
                <div class="form-group">
                  <label for="name" class="sr-only">Name</label>
                  <input type="text" class="form-control form-control-lg" id="name"
                         placeholder="Enter name" v-model="formData.name">
                </div>
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
                <button type="submit" class="btn btn-primary">Submit</button>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "SignUp",
    data() {
      return {
        formData: {}
      }
    },
    methods: {
      submitSignup() {

      }
    }
  }
</script>

<style scoped>

</style>
