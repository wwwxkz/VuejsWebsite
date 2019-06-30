<template>
  <div class="wrapper">
    <!-- Navbar -->
    <div class="header">
      <router-link style="color: #b7b6ba;" to="/">Home</router-link>
      <router-link style="color: #b7b6ba;" to="/About">About</router-link>
    </div>
    <!-- Site body -->
      <div class="main">
        <div class="contact">
          <h2> i'm on github dasdadasdasdadasdaadasdadasdad
            dadasdadasdadasdsdasdasd
            asdadasda
          </h2>
          <h4>Email: contato.wxkz@gmail.com</h4>
          <a href="https://github.com/wxkz">GitHub</a>
          <a href="https://ca.linkedin.com/in/marcelo-rodrigues-campos-5b338418a?trk=people-guest_profile-result-card_result-card_full-click">Linkedin</a>
        </div>
      </div>
  </div>
</template>

<style scoped>
h1, h2, h3, h4, a {
  color: #b7b6ba;
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
  background: rgba(0, 67, 92, 0.8);
}

.main {
  margin: 10px;
  border-style: ridge;
  text-align: left;
  background: rgba(0, 67, 92, 0.4);
}

@media all and (min-width: 800px) {
  .main    { flex: 3 0px; }
  .main    { order: 1; }
}

body {
  padding: 2em; 
}
</style>
