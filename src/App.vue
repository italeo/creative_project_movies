<template>
  <header>
    <router-link to="/">
      <h1><span>FishTale</span>Movies</h1>
    </router-link>
  </header>
   <router-link to="/about">
    <h3 class="about">About</h3>
    </router-link>
    <router-link to="/favorite">
    <h3 class="fav">Favorties</h3>
    </router-link>
  <main>
    <router-view />
  </main>
  <footer>
    <a href="">{{ footerText }}</a>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      footerText: 'GITHUB'
    }
  }

}
</script>


<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;

  &::selection {
    background: transparentize(#42B883, 0.5);
  }
}

body {
  background-color: #35495E;
  padding-top: 50px;
}

a {
  text-decoration: none;
}

header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #2C3D4E;
  box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);

  h1 {
    color: #FFF;
    font-size: 28px;

    span {
      color: #42B883;
    }
  }
}

footer {
  background-color: lightcyan;
  padding: 10px;
  text-align: center;
}
.about {
  color: #FFF;
  text-align: left;
}
.fav {
  color: #FFF;
  text-align: left;
  padding-bottom: 100px;
  
}
</style>