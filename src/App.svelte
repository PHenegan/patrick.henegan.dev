<script lang="ts">
  import { Router, Route } from 'svelte-routing'
  import Home from './pages/Home.svelte'
  import ProjectPage from './pages/ProjectPage.svelte'
  import Header from './lib/Header.svelte'

  export let url = "";
</script>
<Header/>
<div class = "app">
  <Router {url}>
    <Route path = "/"><Home/></Route>
    <Route path = "/projects"><ProjectPage/></Route>
    <Route path = "/test">
      <div>Hello {@html "<Home/>"}</div>
    </Route>
  </Router>
</div>

<style>
  .app {
    padding: 0em 2em;
  }
</style>
