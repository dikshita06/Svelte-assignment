<script>
    import {Column, Row, Button, Tabs, Tab, TabContent, Tag } from "carbon-components-svelte";
    import "carbon-components-svelte/css/all.css";
    import "./index.css"
</script>

<main class="zindex">
    <Row>
        <Column><h1>Contact Us</h1></Column>
    </Row>
    <Row class="details">
        <Column><Tag type="red">ADDRESS</Tag></Column>
        <Column><Tag type="blue">PHONE</Tag></Column>
        <Column><Tag type="cyan">EMAIL</Tag></Column>
    </Row>
    <Row class="contactmargin">
        <Column><h5>27 13 Lowe Haven</h5></Column>
        <Column><h5>111 343 43 43</h5></Column>
        <Column><h5>business@info.com</h5></Column>
    </Row>
</main>