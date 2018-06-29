<template>
<div class="bandejamensajes size">
    <div class="usuario">
      
            <div class="foto">
                <img src="../assets/recursos/foto-01.png" style="border-radius: 50%;">
                <div class="punto"></div>
            </div>
            <div class="nombre">
                <p>Jose Rivero</p>
            </div>

    </div>
    <div class="contenido">
        <div class="con">
            <div class="cont">
                <div class="mensajes">
                    <p>Jueves 28 de junio 23:20</p>
                </div>
                <div class="mensajes mensaje-recibido">
                    <p>Acudo a Uds. porque tengo un problema que me parece que se puede solucionar por customizing...
                </p>
                </div>
                <div class="mensajes mensaje-recibido">
                    <p>Atento a su respuesta</p>
                </div>
                <div class="mensajes mensaje-enviado">
                    <p>Atento a su respuesta</p>
                </div>
                <div class="mensajes mensaje-recibido">
                    <p>Acudo a Uds. porque tengo un problema que me parece que se puede solucionar por customizing...
                </p>
                </div>
                <div class="mensajes mensaje-enviado">
                    <p>Atento a su respuesta</p>
                </div>
                <div class="mensajes mensaje-enviado">
                    <p>Acudo a Uds. porque tengo un problema que me parece que se puede solucionar por customizing...
                </p>
                </div>
            </div>
        </div>
    </div>
    <div class="escribir">
        <div class="mensseger columns ">
            <div class="img column is-2-mobile"><img src="../assets/recursos/foto-01.png" style="border-radius: 50%;" width="35px" height="35px"></div>
            <div class="msg column is-10-mobile">
                <textarea placeholder="Escribe un mensaje"></textarea>
                <div class="iconos-action">
                    <a href="javascript:void(0)" class="item"><img src="../assets/mensajes/icon-adjunto.png" width="25px" height="35px"></a>
                    <a href="javascript:void(0)" class="item"><img src="../assets/mensajes/icon-emoticons.png" width="25px" height="35px"></a>
                    <a href="javascript:void(0)" class="item"><img src="../assets/mensajes/icon-respuesta-guardada.png" width="25px" height="18px"></a>
                    <a href="javascript:void(0)" class="item"><img src="../assets/mensajes/Artboard – 46.png" width="25px" height="18px"></a>
                    
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
.bandejamensajes{
    position: relative;
    font-family: Arial, Helvetica, sans-serif;
}
.usuario{
    //right: -17px;
    //margin-top: 10px; 
    margin-left: 28px;
    display: flex;
    position: relative;
    align-items: center; 
    height: 61px;
    //justify-content: space-around;
}
.foto{
    filter:drop-shadow(0px 15px 10px rgba(0,0,0,0.3));
    //overflow: hidden;
    width: 52px;
    height: 45px;
    position: absolute;
  
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
    top: 39px;
    left: 43px;
}
.nombre
{
    font-size: 16px;
    color: $gris;
    font-weight: bold;
    position: absolute;
    left: 67px;
}
.contenido{
    position: absolute;
  

}
.mensajes{
    position: relative;
    //height: 50px;
    margin-top: 10px;
    color: $gris;
    font-size: 12px;
    &.mensaje-recibido{
        width: auto;
        height: auto ;
        font-size: 13px;
        border-radius: 6px;
        background: $degradado;
        color: $blanco;
        text-align: justify;
        max-width: 84%;  
        padding: 15px 15px 15px 15px;
        //display:inline-block;
        float: left;
        clear: both;
    }
    &.mensaje-enviado{
        width: auto;
        height: auto;
        font-size: 13px;
        border-radius: 6px;
        background: #efefef;
        text-align: justify;
        max-width: 84%;
        padding: 15px 15px 15px 15px;
        float: right;  
        color: $gris;
        clear: both; 
        margin-right: 26px;
    }
}
.escribir{
  position: absolute;
  bottom: 0;
  width: 100%;
  
  //height: 50px;
}
.mensseger{
    float: left;
    width: 100%;
    align-items: center;
    padding: 10px;
    height: 110px;
    display: flex;
    
}
textarea{
    width: 70%;
    //height: 42px;
    border: none;
    outline: none;
    resize: none;
    float: left;
    //margin: 0 0 28px 18px;
    background: #efefef;
}
.iconos-action{
    display: flex;
    background:transparent ;
    align-items: center;
}
.item{
        margin: 0 5px;
}
.msg{
    background: #efefef;
    border-radius: 6px;
}
.cont{
    position: relative;
    height: 56vh;
    overflow: hidden;
    overflow-y: scroll;
    right: -17px;
}
.con{
    top:10px;
    overflow: hidden;
    right: 9px;
    position: relative;
}
</style>


