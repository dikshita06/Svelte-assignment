<script>
    import {Column, Row, Button, TextInput, PasswordInput, Form } from "carbon-components-svelte";
    import "carbon-components-svelte/css/all.css";
    import "./index.css";
    import { navigate } from "svelte-routing";
    // import "./store"
    let data
    let user
    let password
    let username
    function loginfunc() {
    event.preventDefault();
    username = "abc";
    password = "12345";
     localStorage.setItem('name',username);
    // data = JSON.parse(user);
    localStorage.setItem('password', password)

}

</script>

<main class="display">
    <Form on:submit = {loginfunc} >
     <Row>
        <Column><div class="pagename">
            <h1>Login</h1>
        </div></Column>
    </Row>
    <Row>
        
        <Column><TextInput bind:value={username} labelText="User name" placeholder="Enter user name" /></Column>
        <Column><PasswordInput bind:value={password} labelText="Password" placeholder="Enter password" /></Column>
        
    
    </Row>
    <Row>
        <Column><Button type="submit" on:click={() => navigate ("/")}>Log In</Button></Column>
    </Row>
</Form>
    
</main>