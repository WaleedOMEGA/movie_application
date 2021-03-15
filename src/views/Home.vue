<template>
  <div class="home">
    <navbar />
    <div id="main-section">
      <sidebar />
      <movie-list />
    </div>
  </div>
</template>

<script>
import Sidebar from "../components/Sidebar";
// @ is an alias to /src
import Navbar from "../components/Navbar";
import MovieList from "../components/MovieList";
export default {
  name: "Home",
  components: {
    Navbar,
    Sidebar,
    MovieList
  }
};
</script>
<style lang="scss" scoped>
.home {
  display: flex;
  flex-direction: column;

  #main-section {
    display: flex;
    margin-top: 50px;
  }
}
</style>
