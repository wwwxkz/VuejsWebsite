<template>
  <div class="home">
    <!-- Navbar -->
    <div class="navbar">
      <router-link to="/">Home</router-link>
      <router-link to="/About">About</router-link>
    </div>
    <!-- Site body -->
    <div class="about">
      <h2>Teste</h2>
      <h4>So perhaps, you've generated some fancy text, and you're content that you can
       now copy and paste your fancy text in the comments section of funny cat videos, but
       perhaps you're wondering how it's even possible to change the font of your text? Is
       it some sort of hack? Are you copying and pasting an actual font?
      </h4>
      <br>
      <h2>My Skills</h2>
      <h4>
        Python... now copy and paste your fancy text in the comments section of funny cat videos, 
        but perhaps you're wondering how it's even possible to change the font of your text? Is
        it some sort of hack? Are you copying and pasting an actual font?
      </h4>
      <img src="../assets/shaggy.gif">
    </div>
  </div>
</template>

<style scoped>
div {
  border-style: ridge;
  background-color: pink;
  box-shadow: 1px 1px 10px black;
}

h1, h2 {
  font-weight: normal;
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
