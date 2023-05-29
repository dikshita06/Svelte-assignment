<script>
  import { Router, Route } from 'svelte-routing'
  import Home from './home.svelte'
  import Login from './login.svelte';
  import Signup from './signup.svelte';
  import About from './about.svelte';
  import Contact from './contact.svelte';
  
</script>

<Router>
  <Route path="/">
    <Home /></Route>
    <Route path="/login" component={Login} />
    <Route path="/signup" component={Signup} />
    <Route path="/about" component={About} />
    <Route path="/contact" component={Contact} />
</Router>