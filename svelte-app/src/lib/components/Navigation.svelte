<nav>
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
</nav>

<script>
    let isOpen = false; //Hamburger open or closed definition
</script>

<nav class = "nav">
    <button class = "burger" on:click={() => isOpen =! isOpen} aria-label="Toggle navigation">
        </button>


        <ul class:open={isOpen}>
        <li><a href = "/">Home</a></li>
        <li><a href = "/about">About</a></li>
        <li><a href = "/contact">Contact</a></li>
    </ul>
</nav>

<style>
.nav {
    background-color: #007bff;
    padding: 1rem;
    text-align: center;
}
nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    text-decoration: none;
    color: white;
    font-weight: bold;
}

.burger{
    display: none;
    font-size: 2rem;
    background: none;
    border: none;
    cursor: pointer;
    color: white;
    position: absolute;
    top: 1rem;
    left: 1rem;
}

    @media (max-width: 768px){
        .burger {
            display: block;
        }
    }
</style>
