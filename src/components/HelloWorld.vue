<template>
  <div>
    <b-navbar toggleable type="dark" variant="dark">
      <b-navbar-brand href="#">NavBar</b-navbar-brand>

      <b-navbar-toggle target="navbar-toggle-collapse">
        <template #default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
          <b-icon v-else icon="chevron-bar-down"></b-icon>
        </template>
      </b-navbar-toggle>

      <b-collapse id="navbar-toggle-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#">Link 1</b-nav-item>
          <b-nav-item href="#">Link 2</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
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
