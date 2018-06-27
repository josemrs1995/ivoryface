<template>
    <div class="bandeja">
        <div>
            <a class="boton s">Nuevo mensaje</a>
        </div>
        <div class="icono img">
             <p><img src="../assets/Mensajes/icon-usuarios.png" width="18px" height="18 px"></p>
        </div>
        <div class="icono busqueda">
             <p><img src="../assets/Mensajes/icon-busqueda.png" width="18px" height="18 px"></p>
        </div>
        <div class="icono letra">
            <p> Todo</p>
        </div>
        <div class="icono letra-2">
            <p>Bandeja de entrada</p>
        </div>
        <div class="cont">
            
            <div class="mensajes">
                <div class="caja msj ">
                     <div class="red"><img src="../assets/Recursos/logo-twitter-degradado.png" width="18px" height="18 px" style="cursor:pointer;"></div>
                    <div class="cajita foto ">
                    <img src="../assets/recursos/foto-01.png" style="border-radius: 50%;">
                    <div class="punto"></div>
                    </div>
                    <div class="cajita contenido">
                        <p> Jose Rivero </p>
                        <p class="mensajito">hola como estas</p>
                        <!--<div class="boton ss"><img src="../assets/Mensajes/icon-imagen.png" width="18px" height="18 px"></div>
                        <div class="boton ss"><img src="../assets/Mensajes/icon-imagen.png" width="18px" height="18 px"></div>-->
                    </div>
                    <div class="border-left">
                        <div class="extras">
                            <img src="../assets/Mensajes/icon-marcar-leido.png" width="14px" height="14px" style="cursor:pointer;">
                            <img src="../assets/Mensajes/icon-eliminar.png" width="10px" height="10px" style="cursor:pointer;">
                            <img src="../assets/Mensajes/icon-posponer.png" width="14px" height="14px" style="cursor:pointer;">
                        </div>
                    </div>
                </div>
                <div class="caja msj ">
                     <div class="red"><img src="../assets/Recursos/logo-facebook-degradado.png" width="18px" height="18 px" style="cursor:pointer;"></div>
                    <div class="cajita foto ">
                    <img src="../assets/recursos/foto-01.png" style="border-radius: 50%;">
                    <div class="punto"></div>
                    </div>
                    <div class="cajita contenido">
                        <p> Jose Rivero </p>
                        <p class="mensajito">hola como estas</p>
                        <!--<div class="boton ss"><img src="../assets/Mensajes/icon-imagen.png" width="18px" height="18 px"></div>
                        <div class="boton ss"><img src="../assets/Mensajes/icon-imagen.png" width="18px" height="18 px"></div>-->
                    </div>
                    <div class="border-left">
                        <div class="extras">
                            <img src="../assets/Mensajes/icon-marcar-leido.png" width="14px" height="14px" style="cursor:pointer;">
                            <img src="../assets/Mensajes/icon-eliminar.png" width="10px" height="10px" style="cursor:pointer;">
                            <img src="../assets/Mensajes/icon-posponer.png" width="14px" height="14px" style="cursor:pointer;">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
$blanco:#fff;
$negro:#000;
$gris:#8F8F8F;
$azul:#1F8EFA;
$verdea:#75EAFF;
$degradado:linear-gradient(45deg, rgba(77,166,254,1) 0%, rgba(0,228,253,1) 100%);
$grisc:#D3D3D3;
.bandeja{
    position: relative;
    width: 100%;
}
.boton{
    text-decoration: none;
    width: 35px;
    height: 35px ;
    border-radius: 40px;
    font-size: 20px;
    background: $degradado;
    color: $blanco;
    font-weight:normal;
    //transform: translate(40px, 51px);
    //opacity:1;
    display: flex;
    justify-content: center;
    align-items: center;
    //position: absolute;
        &.s{
            width: 113px;
            height: 35px ;
            font-size: 10px;
            transform: translate(22px, 15px);
            border-radius: 6px;
            position: absolute;
        
        }
         &.ss{
            width: 66px;
            height: 20px;
            font-size: 10px;
            //border-radius: 6px;

         }

}
.icono{
    width: 35px;
    height: 35px ;
    border-radius: 50%;
    font-size: 20px;
    background: $degradado;
    color: $blanco;
    font-size: 20px;
    font-weight:normal;
    transform: translate(-19px, 19px);
    opacity:1;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
      &.img{
        background: transparent;
        position: absolute;
        top: 49px;
        left: 35px;
     }
     &.busqueda{
        background: transparent;
        transform: translate(49px, 78px);
        width: 18px;
        height: 18px ;
     }
     &.letra{
        position: absolute;
        background: transparent;
        //transform: translate(210px, 50px);
        color:$grisc;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 14px;
        top: 48px;
        right: -12px;
     }
      &.letra-2{
        position: absolute;
        background: transparent;
        //transform: translate(-232px, 85px);
        color:$gris;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 14px;
        width: 139px;
        top: 80px;
        left: 33px;
        font-weight: bold;
     }
}
.mensajes{
    height: 55vh;
    overflow: hidden;
    overflow-y: scroll;  
    position: relative;
    right: -17px;
}
.cont{
    transform:translate(0px,117px);
    overflow: hidden;
    right: 9px;
    position: relative
}
.foto{
    filter:drop-shadow(0px 15px 10px rgba(0,0,0,0.3));
    overflow: hidden;
    width: 45px;
    height: 45px;
    position: relative;
    /*top: 15px;
    left: 15px;*/
     //transform: translate(-113px, 18px);
}
.punto{
    height: 10px;
    width:10px;
    background: #00BD43;
    font-size: 100px;
    border-radius: 50px;
    //transform: translate(40px, 40px);
    overflow: hidden;
    position: absolute;
    top: 32px;
    left: 33px;
}
.caja{
    height: 100px;
    width: 100%;
    //border:solid;
    //transform: translate(-4px,127px);
    margin-top: 10px; 
    display: flex;
    justify-content: space-around;
    align-items: center; 
    position: relative;
}
.cajita{
    max-width: 65%;
    text-align: left;
    font-weight: bold;
    color: $gris;
    &.contenido{
        width: 95%
    }
}
.mensajito{
        font-weight: normal;
}
.red{
    top: 17px;
    right: 35px;
    position: absolute
}
.extras{
    background: #75EAFF;
    height: 80px;
    width: 20px;
    display: flex;
    flex-direction: column;
    position: relative;
    top: 10px;
    align-items: center;
    justify-content: space-around;

}
.border-left{
    border-left: #75EAFF solid;
    height: 100%; 
    visibility: hidden;
}
.caja:hover .border-left {
    visibility: visible;
}
  
</style>


