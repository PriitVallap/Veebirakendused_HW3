<template>
  <body>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab&display=swap" rel="stylesheet">
    <header>
      <nav>
        <div class="logo-container">
          <img src="./images/logo.png" alt="postIt">
        </div>
        <div class="search-container">
          <input type="text" name="search"><button type="button">Search</button>
        </div>
        <div class="avatar-container">
          <img class="avatar">
          <div class="drop-down-container">
            <span id="user-name">John Doe</span>
            <span id="user-email"></span>
            <span class="separator"></span>
            <span>
              <a href="Browse.Vue">Browse</a>
            </span>
            <span class="separator"></span>
            <span>
              <a href="Login.Vue">Log Out</a>
            </span>
          </div>
        </div>
      </nav>
    </header>
    <section class="main-container"></section>
  </body>
</template>

<script>
export default {
  name: 'Index',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./style.css">
</style>
