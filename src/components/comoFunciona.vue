<template>
    <section>
        <div class="overlay"></div>
        <div class="container">
            <div class="row">
                <div class="col-md-12 text-center">
                    <h2>¿Como funciona {{name}}?</h2>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4">
                    <img src="../assets/wall-calendar.png" alt="">
                    <h4>AGENDA</h4>
                    <p>Selecciona tus servicios, horario y fecha de tu cita</p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/credit-card.png" alt="">
                    <h4>CONFIRMA</h4>
                    <p>Ingresa tus datos y paga en línea</p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/brush.svg" alt="">
                    <h4>RECIBE</h4>
                    <p>Recibe a tu Espscialista {{name}}</p>
                </div>
            </div>
        </div>
    </section>
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
    section{
        background-attachment: fixed;
        background-image: url('.././assets/d.jpg');
        width: 100%;
        min-height: 600px;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    }

    .overlay{
        background-color: #222534;
        position: absolute;
        top: 0;
        left: 0;
        display: block;
        width: 100%;
        height: 100%;
        opacity: 0.6;
        filter: alpha(opacity=40);
        z-index: 0;
    }

    h2{
        margin-top:80px;
        color:#fff;
        font-size: 40px;
    }

    img{
        max-width: 100px;
        margin-top:100px;
        margin-bottom: 40px;
    }
    h4{
        color: #fff;
        margin-bottom: 20px;
    }
    p{
        color: #fff;
        letter-spacing: 1.5px;
    }
</style>
