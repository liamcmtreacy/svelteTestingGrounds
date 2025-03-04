<script> 
    import {onMount} from 'svelte';

    onMount(() => {
        console.log("About Page Loaded");
    })
</script>

<h1> Get in Contact With Us </h1>
<p> Get in touch via email, <a href = "mailto:info@example.ie">info@example.com</a>.</p>


<style>
    h1{color: #007bff;}
    p {font-size: 18px;}
    a {color: #007bff; text-decoration: none;}
    a:hover {text-decoration: underline;}
</style>
