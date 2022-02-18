<template>
    <header>
        <img :src="require('@/assets/images/logo.png')" alt="">
        <ul>
            <li><a href="/colares">Colares</a></li>
            <li><a href="/brincos">Brincos</a></li>
            <li><a href="/pulseiras">Pulseiras</a></li>
            <li><a href="/aneis">Anéis</a></li>
        </ul>
    </header>

    <div id="main">
        <img :src="require('@/assets/images/logo verao.jpg')" alt="">
    </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    header {
        background: #ffeffd;
        width: 100%;
        box-shadow: 2px 3px 5px black;
    }

    header img {
        width: 150px;
        height: fit-content;
    }

    ul {
        display: inline-block;
        position: absolute;
        margin: 70px auto;
        width: 80%;
    }

    li {
        list-style: none;
        display: inline-block;
        width: 25%;
        height: 100%;
        text-align: center;
    }

    a {
        padding: 0 30% 0 30%;
        width: 100%;
        color: black;
        text-decoration: none;
    }

    li:hover {
        cursor: pointer;
        transition: ease 1s;
    }

    li:hover a {   
        text-decoration: underline;
    }

    #main img {
        width: 90%;
        margin: 40px auto;
        display: block;
        height: fit-content;
        border-radius: 12px;
    }

</style>