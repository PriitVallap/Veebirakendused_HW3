<template>
  <body>
    <header>
      <nav>
        <div class="logo-container">
          <img src="./images/logo.png" alt="postIt">
        </div>
        <div class="search-container">
          <input type="text" name="search"><button type="button">Search</button>
        </div>
        <Dropdown></Dropdown>
      </nav>
    </header>
    <section class="main-container"></section>
  </body>
</template>

<script>
import Dropdown from "@/components/Dropdown";
export default {
  name: 'Browse',
  components: {Dropdown},
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./style.css">
</style>
