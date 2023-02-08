<template>
    <div class="stats-box">
        <h3>Estatísticas</h3>
        <div class="stats">
            <h4>Total de Usuários na Plataforma: {{ users }}</h4>
            <h4>Média de acessos diários: {{ averagePerDay }}</h4>
        </div>
        <button>Ver Detalhes</button>
    </div>
</template>

<script>

export default ({
    data() {
        return{
            users: 139,
            averagePerDay: 20
        }
    }
})
</script>

<style scoped>
.stats-box {
    color: #ffff;
    background-color: #21222c;
    padding: 20px;
    margin: 50px;
    border-radius: 20px;
    box-shadow: 10px 5px 5px #222222;
}

.stats{
   color: darkgray;
   margin-top: 20px;
}

h4{
   color: darkgray;
   margin-bottom: 10px;
}

button {
    background-color: #6E46A4;
    color: #fff;
    margin-top: 10px;
    padding: 10px;
    border: none;
    border-radius: 10px;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

button:hover {
    background-color: #4c2f72;
    transition: all ease-in-out 250ms;
}

</style>
