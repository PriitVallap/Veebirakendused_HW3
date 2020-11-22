<template>
  <div class="avatar-container">
    <a href="#" v-on:click.prevent="showDropDown=!showDropDown">
      <img class="avatar">
    </a>
    <transition name="slide-fade">
      <div v-if="showDropDown">
        <span v-for="l in links" class="list">
          <div v-if=l.link.includes("user")>
          <p class={{l.link}}}>{{l.name}}}</p>
          </div>
          <div v-else>
            <a href={{l.link}}>{{l.name}}</a>
          </div>
        </span>
      </div>
    </transition>
  </div>
</template>

<script>
import Browse from "@/components/Browse";
import Login from "@/components/Login";

export default {
  name: 'Dropdown',
  data() {
    return {
      showDropDown: false,
      links: [
        {link: 'user-name',name:"John Doe"},
        {link: 'user-email',name:"e-mail"},
        {link: Browse,name: "Browse"},
        {link: Login,name: "Logout"}
      ]
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
