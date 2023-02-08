<template>
    <div class="box">
        <div class="title">
            <h3>Projetos Recentes</h3>
        </div>
        <div class="project">
            <img src="../assets/text-editor.png" alt="">
            <div class="infos">
                <h4>Nome do projeto: {{ projectName }}</h4>
                <h4 class="description">Descrição</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec porta, purus non rutrum facilisis, arcu massa blandit nulla, a sollicitudin nunc enim a arcu. Morbi sit amet volutpat risus. Aenean...</p>
            </div>
        </div>
    </div>
</template>

<script>

export default ({
    data() {
        return{
            projectName: "text-editor"
        }
    }
      
    
})
</script>

<style scoped>
.box {
    color: #ffff;
    background-color: #21222c;
    border-radius: 20px;
    padding: 50px;
    margin: 50px;
    box-shadow: 10px 5px 5px #222222;
}

.title {
    margin-bottom: 20px;
}

.project img{
    width: 10vw;
    height: 10vh;
    margin-right: 10px;
}

.project {
    display: flex;
    padding: 10px;
    border-radius: 20px;
}

.project:hover {
    background-color: #6E46A4;
    transition: all ease-in-out 250ms;
}

.infos h4{
    margin-bottom: 10px;
}

.description, .infos p{
    color: darkgray;
}

</style>
