<template>
    <header class="header">

        <div class="header-box">
            <h2 class="title">
                <span>Rock</span>
                <span>Paper</span>
                <span>Scissors</span>
                <span>Lizard</span>
                <span>Spock</span>
            </h2>
            <Score />
        </div>
    </header>
</template>

<script>
    import Score from './Score.vue';

    export default {

        name: 'Header',
        components: {
            Score,
        }
    };

</script>

<style lang="scss" scoped>

.header {

display: flex;
justify-content: center;
align-items: center;
width: 100%;
max-width: 800px;
padding: rfs(30px);

@media (min-width: 800px) {
    margin: 0 auto;
}

&-box {
display:flex;
justify-content: space-between;
align-items: center;
width: 100%;
border: 2px solid $header-outline;
border-radius: 20px;
padding: rfs(20px 30px);

.title {
display: flex;
flex-direction: column;
line-height: 0.8em;
color: $scissors-to;
font-size: 2rem;

}

}

}

</style>