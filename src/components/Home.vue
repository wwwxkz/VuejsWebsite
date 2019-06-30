<template>
  <div class="wrapper">
    <!-- Navbar -->
    <div class="header">
      <router-link style="color: #b7b6ba;" to="/">Home</router-link>
      <router-link style="color: #b7b6ba;" to="/About">About</router-link>
    </div>
    <!-- Site body -->
      <div class="main">
        <div class="about">
          <h2>I'm</h2>
          <h4>So perhaps, you've generated some fancy text, and you're content that you can
          now copy and paste your fancy text in the comments section of funny cat videos, but
          perhaps you're wondering how it's even possible to change the font of your text? Is
          it some sort of hack? Are you copying and pasting an actual font?
          </h4>
          <br>
        </div>
        <div class="projects">
          <h2>My Projects</h2>
          <h4>api results here</h4>
        </div>
      </div>
      <div class="secondary">
        <div class="skills">
          <h2>My Skills</h2>
          <h4>
            Python... now copy and paste your fancy text in the comments section of funny cat videos, 
            but perhaps you're wondering how it's even possible to change the font of your text? Is
            it some sort of hack? Are you copying and pasting an actual font?
          </h4>
          <img src="../assets/shaggy.gif">
        </div>
      </div>
  </div>
</template>

<style scoped>
h1, h2, h3, h4 {
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

.secondary {
  margin: 10px;
  border-style: ridge;
  background: rgba(0, 67, 92, 0.4);
}

@media all and (min-width: 600px) {
  .secondary { flex: 1 0 0; }
}

@media all and (min-width: 800px) {
  .main    { flex: 3 0px; }
  .main    { order: 1; }
  .secondary { order: 2; }
}

body {
  padding: 2em; 
}
</style>
