<template>
<body>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab&display=swap" rel="stylesheet">
    <section class="login-page">
      <section id="login-container">
        
        <div>
          <h1>Welcome to postIt!</h1>
        </div>
        <div>
          <h4>
            <a href="#">Create an Account</a>
          </h4>
        </div>
        <div>
          <h4>Or</h4>
        </div>
        <div>
          <h3>Please Log In</h3>
          <form action="index">
            <div>
              <input type="text" name="email" placeholder="Email">
            </div>
            <div>
              <input type="password" name="password" placeholder="Password">
            </div>
            <div>
              <router-link to="/index">
              <button @click="go_to_index" type="button">Log In</button>
              </router-link>
            </div>
            <div>
              <small>
                <a href="#">Forgot password?</a>
              </small>
            </div>
          </form>
        </div>
      </section>
    </section>
</body>
  
</template>

<script>
export default {
  name: 'Login',
  props: {
    msg: String
  },
  methods: {
    go_to_index: function() {
      this.$router.push("/index")
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./style.css">
</style>
