<script>
    import {Column, Row, Button,} from "carbon-components-svelte";
    import "carbon-components-svelte/css/all.css";
    import "./index.css";
    import About from "./about.svelte";
    import Contact from "./contact.svelte";
    import { Router, Link, Route} from "svelte-routing";
    import Login from "./login.svelte";
    import Signup from "./signup.svelte";
    import { navigate } from 'svelte-routing'
</script>

<main>
   <Row>
       <Column><div class= "website">
           <h2>Equal Point Web Design</h2>
           <h4>Websites Done Differently</h4>
       </div></Column>
       <Column> <nav>
        <Link style="margin-right:25px" to="/about">About us</Link>
        <Link to="/contact">Contact Us</Link>
    </nav>
    </Column>
   </Row>
   <Row>
       <Column><h1>Bespoke Web Design For The Small Business</h1></Column>
       <Column></Column>
   </Row>
   <Row>
       <Column><p>Bespoke Website development for the small business. We build modern, fast and SEO friendly websites using the lastest trends. We focus on helping you attract more visitors and improve your business.</p></Column>
       <Column></Column>
   </Row>
   <Row>
    <Column><div class="click">
        <Button on:click={() => navigate("/login")} >Login</Button>
        <Button on:click={() => navigate("/signup")} >Sign Up</Button>
    </div></Column>
    <Column></Column>
   </Row>
</main>
