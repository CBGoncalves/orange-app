<template>
    <div class="nav">
        <nav>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/">Explorar</a></li>
                <li><a href="/">Meus Projetos</a></li>
                <li><a href="/">Sobre</a></li>
                <li v-=user><a href="/">Estatísticas</a></li>
                <li style="float: right"><a class="active" href="#user">{{ name }}</a></li>
            </ul>
        </nav>
    </div>
</template>

<script>

export default ({
    setup() {
        
    },
    data() {
        return{
            name: "Carlos",
            user: false
        }
    }
})
</script>

<style scoped>
    li a {
        display: block;
        color: white;
        text-decoration: none;
        text-align: center;
        padding: 20px 16px;
    }
    li {
        float: left;
    }
    ul {
        list-style-type: none;
        margin: 7px;
        padding: 0;
        overflow: hidden;
        background-color: #21222c;
        border-radius: 20px;
    }
    li a:hover{
        background-color: #6E46A4;
        color: #ffff;
        transition: all ease-in-out 250ms;
    }
    .active {
        background-color: #6E46A4;
    }
</style>
