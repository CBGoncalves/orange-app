<template class="template">
  <NavigationBar />
  <div class="main">
    <WelcomeMessage />
    <StatsWindow />
  </div>
  <ProjectWindow />
</template>

<script>
import NavigationBar from './components/NavigationBar.vue';
import WelcomeMessage from './components/WelcomeMessage.vue';
import ProjectWindow from './components/ProjectsWindow.vue';
import StatsWindow from './components/StatsWindow.vue'

export default {
  name: 'App',
  components: {
    NavigationBar,
    WelcomeMessage,
    ProjectWindow,
    StatsWindow
  },
  data() {
    return {
      name: "Carlos"
    }
  }
}
</script>

<style>
* {
  margin: 0;
}

body {
  background-color: #282a36;
}

#app {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.main {
  display: flex;
  justify-content: center;
}
</style>
