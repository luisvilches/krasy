<template>
    <div class="postfooter">
        <ul>
            <li>{{name}}  © Copyright todos lo derechos reservados</li>
            <li> | </li>
            <li>Hecho con <i class="fas fa-heart"></i></li>
        </ul>
    </div>    
</template>

<script>
export default {
    data(){
        return {
            name:'Krasy'
        }
    },
}
</script>

<style scoped>
    ul li{
        display: inline-block;
        list-style: none;
        color: #fff;
    }

    .postfooter{
        padding: 10px 0px 1px 0px;
        background: #222;
    }
</style>
