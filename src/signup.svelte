<script>
    import {Column, Row, Button, TextInput, Form } from "carbon-components-svelte";
    import "carbon-components-svelte/css/all.css";
    import "./index.css";
    import { navigate } from "svelte-routing";
    let username
    let password
    let email
    let valid = true
    function signupfunc() {
    event.preventDefault();
    username = "abc";
    password = "12345";
    email = "abc@gamil.com"
     localStorage.setItem('name',username);
    // data = JSON.parse(user);
    localStorage.setItem('password', password)
    localStorage.setItem('email', email)

}
</script>



<main class="register">
    <Form on:submit = {signupfunc} >
    <Row>
        <Column><div class="tag">
            <h1>Sign Up</h1>
        </div></Column>
    </Row>
    <Row>
        <Column><TextInput labelText="Username" placeholder="Username" /></Column>
        <Column><TextInput labelText="Email" placeholder="Email" /></Column>
        <Column><TextInput labelText="Password" placeholder="Password" /></Column>
    </Row>
    <Row>
        <Column><Button type="submit"on:click={() => navigate("/")}>Sign Up</Button></Column>
    </Row>
</Form>
</main>