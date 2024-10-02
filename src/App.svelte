<script>
  import { Router, Link, Route } from "svelte-routing";
  export let url = "";
</script>

<Router {url}>
  <nav>
    <Link to="/">Home</Link>
    <Link to="/about">About</Link>
  </nav>
  <div>
    <Route path="/about">About</Route>
    <Route path="/">Home</Route>
  </div>
</Router>
