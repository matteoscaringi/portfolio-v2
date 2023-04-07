<script lang="ts">
    import index from "../../../public/index.jpg";
    import Icon from '@iconify/svelte';
</script>

<main class="hero">
    <img src={index} alt="Matteo Scaringi" class="image" />
    <header class="herotext">
        <p class="font-light">Hello! I'm</p>
        <p class="font-bold">Matteo Scaringi</p>
    </header>
    <header>
        <a href=""><Icon icon="simple-icons:github" color="black" /></a>
        <a href=""><Icon icon="simple-icons:twitter" color="black" /></a>
    </header>
</main>

<style lang="scss">
    /*Imports*/
    @import url('https://fonts.googleapis.com/css2?family=Roboto+Flex:wght@300;700&display=swap');

    /*General content properties*/
    .hero{
        /*set vertical position to be in the middle*/
        display: flex;
        flex-direction: column;
        align-items: center;
        
        justify-content: center;
        text-align: center;
    }
    .herotext {
        line-height: 5px;
    }
    .image {
        width: 250px;
        height: 250px;
        border-radius: 10%;
    }

    /*Specific content properties*/
    .font-bold {
        font-family: 'Roboto Flex', sans-serif;
        font-weight: bold;
    }
    .font-light {
        font-family: 'Roboto Flex', sans-serif;
        font-weight: lighter;
    }
</style>
