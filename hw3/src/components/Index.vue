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
        <Dropdown></Dropdown>
      </nav>
    </header>
    <section class="main-container"></section>
  </body>
</template>

<script>
import router from './router'
import Dropdown from "@/components/Dropdown";
export default {

        name: 'Index',
  components: {Dropdown},
  data () {
            return {
                msg: '123'
            }
        },
        methods: {
            navigate() {
                router.push({ name: "login" });
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./style.css">
</style>
