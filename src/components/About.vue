<template>
  <div class="wrapper">
    <!-- Navbar -->
    <div class="header">
      <ul>
        <li>
          <router-link class="router" to="/">Home</router-link>
        </li>
        <li>
          <router-link class="router" to="/About">About</router-link>
        </li>
      </ul>
    </div>
    <!-- Site body -->
      <div class="main">
        <div class="contact">
          <h2>Send me a message at contato.wxkz@gmail.com, or you can also find me at <a href="https://github.com/wxkz">GitHub</a> and <a href="https://ca.linkedin.com/in/marcelo-rodrigues-campos-5b338418a?trk=people-guest_profile-result-card_result-card_full-click">Linkedin</a>.</h2>
        </div>
      </div>
  </div>
</template>

<style scoped>
h1, h2, h3, h4, a, li {
  color: white;
}

.wrapper {
  display: flex;  
  flex-flow: row wrap;
  font-weight: bold;
  text-align: center;
}

.wrapper > * {
  padding: 10px;
  flex: 1 100%;
}

.header {
  border-style: ridge;
  border-color: white;
  background: rgba(179, 4, 4, 0.9);
}

.header > ul {
  float: left;
  display: inline-flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
.router {
  display: block;
  color: white;
  text-align: center;
  padding: 14px;
  text-decoration: none;
}
.router:hover {
  background-color:rgba(223, 93, 93, 0.9);
}

.main {
  margin: 10px;
  border-color: white;
  border-style: ridge;
  text-align: left;
  background: rgba(179, 4, 4, 0.8);
}

@media all and (min-width: 800px) {
  .main    { flex: 3 0px; }
  .main    { order: 1; }
}

body {
  padding: 2em; 
}
</style>
