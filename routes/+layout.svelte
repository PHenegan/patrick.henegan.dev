<script>
  let { children } = $props();
</script>

<style>
  .header {
    display: flex;
    justify-content: space-between;
    background-color: #E0E0E0;
  }

  .header-pages > * {
    display: inline-flex;
    justify-content: flex-start;
  }
  .header-links > * {
    display: inline-flex;
    justify-content: flex-end;
  }

  ul {
    flex-direction: row;
  }

</style>

<div class = "header">
  <ul class = "header-pages">
    <li><a href = "/">Home</a></li>
    <li><a href = "/projects">Projects</a></li>
    <li><a href = "/experience">Experience</a></li>
  </ul>
  <ul class = "header-links">
    <li><a href = "https://github.com/PHenegan"> GitHub</li>
    <li><a href = "https://www.linkedin.com/in/patrick-henegan">LinkedIn</li>
  </ul>

</div>

{@render children()}
