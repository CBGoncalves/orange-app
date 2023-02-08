<template>
    <div class="welcome">
        <h2>Bem vindo de volta {{ name }}</h2>
    </div>
</template>

<script>

export default ({
    data(){
        return {
            name: "Carlos"
        }
    }
})
</script>

<style scoped>
.welcome {
    color: #ffff;
    display: flex;
    justify-content: center;
    margin: 70px;
    padding: 50px;
    background-color: #21222c;
    border-radius: 20px;
    box-shadow: 10px 5px 5px #222222;
}

</style>
