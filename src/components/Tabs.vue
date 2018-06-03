<template>
    <section class="container-fluid">
        <div class="row">
            <div class="col-md-12 pd">
                <h2>ELIGE TU SERVICIO DE BELLEZA {{name}}</h2>
            </div>
        </div>
        <div class="row">
            <div class="col-md-12">
                <br>
                <br>
                <ul class="nav nav-pills mb-3 justify-content-center" id="pills-tab" role="tablist">
                    <li class="nav-item">
                        <a class="nav-link active" id="pills-home-tab" data-toggle="pill" href="#pills-home" role="tab" aria-controls="pills-home" aria-selected="true">Manicure / Pedicure</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" id="pills-profile-tab" data-toggle="pill" href="#pills-profile" role="tab" aria-controls="pills-profile" aria-selected="false">Alisado keratina</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" id="pills-contact-tab" data-toggle="pill" href="#pills-contact" role="tab" aria-controls="pills-contact" aria-selected="false">Peluqueria</a>
                    </li>
                </ul>
                <div class="tab-content" id="pills-tabContent">
                    <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">
                        <br>
                        <Pack 
                            title="Servicio de manicure y/o pedicure a domicilio"
                        
                        />
                    </div>
                    <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">
                        <br>
                        <Pack 
                            title="Servicio de alisado keratina a domicilio"
                        />
                    </div>
                    <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">
                        <br>
                        <Pack 
                            title="Servicio de peluqueria a domicilio"
                        />
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Pack from './pack'
export default {
    data(){
        return {
            name:'Krasy'
        }
    },
    components:{
        Pack
    }
}
</script>

<style scoped>
    section{
        min-height: 380px;
    }

    .nav-link{
        background: #fff;
        border:1px solid #eee;
        width: 300px;
        padding: 20px;
        border-radius: 0px;
        color: #341f97;
    }

    @media(max-width:991px){
        .nav-link{
            padding: 20px;
        }
    }

    .nav-link.active{
        border:2px solid #341f97;
        color: #fff;
        background: #341f97;
    }

    .pd{
        padding: 40px 40px 0px 40px;
    }

    h2{
        text-transform: uppercase;
    }
</style>
