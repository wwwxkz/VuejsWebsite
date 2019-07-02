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
        <div class="about">
          <h2>Who is Marcelo ?</h2>
          <h4>Hello, how are you? Ok .. Let's start, my name is marcelo I'm 15 years old on the day i'm
            doing this, in the case 1/7/2019 11:19. I believe that this is not what you want to know, so
            come on, as you can see i know some programming languages and other little things like:
            Maya, zBrush, Photoshop, UnrealEngine 4, Mudbox, 3dsmax, Blender and others. I know these things
            because Iam graduated in Game Development since 2019. I am a guy who does not know how to
            talk about himself even talking a lot "rs", finally I think that's it,if you want to contact me
            go to the about page :)
          </h4>
          <br>
        </div>
        <div class="projects">
          <h2>Projects</h2>
          <div style="margin:10px;background-color:rgba(223, 93, 93, 0.9);border-style:ridge;border-color:white;" v-for="(repository, index) in repositories" :key="index">
            <h3 style="margin:10px;">{{ repository.name }}</h3>
            <h4 style="margin:10px;">{{ repository.description }}</h4>
          </div>
        </div>
      </div>
      <div class="secondary">
        <div class="skills">
          <h2>Skills</h2>
          <div class="languages">
          <h3>Languages</h3>
            <ul>
              <li>
                JavaScript
              </li>
              <li>
                ShellScript
              </li>
              <li>
                Python
              </li>
              <li>
                Java
              </li>
              <li>
                Dart
              </li>
              <li>
                c++
              </li>
              <li>
                c#
              </li>
              <li>
                c
              </li>
            </ul>
          </div>
          <div class="frameworks">
            <h3>Frameworks</h3>
            <ul>
              <li>
                React Native
              </li>
              <li>
                Expressjs
              </li>
              <li>
                Asp.net
              </li>
              <li>
                Flutter
              </li>
              <li>
                Angular
              </li>
              <li>
                Django
              </li>
              <li>
                Vuejs
              </li>
              <li>
                Flask
              </li>
              <li>
                Nodejs
              </li>
              <li>
                Kivy
              </li>
            </ul>
          </div>
          <img src="../assets/shaggy.gif">
        </div>
      </div>
  </div>
</template>

<style scoped>
h1, h2, h3, h4, li {
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
  border-style: ridge;
  border-color: white;
  text-align: left;
  background: rgba(179, 4, 4, 0.8);
}

.secondary {
  display: flex;
  text-align: left;
  margin: 10px;
  border-color: white;
  border-style: ridge;
  background: rgba(179, 4, 4, 0.8);
}
.skills > div {
  display: inline-table;
}
.skills > div > ul > li {
  margin-left: -25px;
  margin-right: 80px;
}

.skills > .framworks > ul > li {
  float: right;
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

<script>
  import axios from 'axios';

  export default {

    date() {
      return {
        repositories: [],
      }
    },

    created(){
      axios.get('https://api.github.com/users/wxkz/repos').then((response) => {
        this.repositories = response.data;
      })
    }
  
  
  }

</script>
