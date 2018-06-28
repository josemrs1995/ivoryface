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
        <div class="mensajes">
            <p>Jueves 28 de junio 23:20</p>
        </div>
        <div class="mensajes mensaje-recibido">
            <p>Acudo a Uds. porque tengo un problema que me parece que se puede solucionar por customizing...
                Sucede que me he encontrado que el sistema está configurado para que se generen mensajes cuando se crean pedidos por la ME21N.
           </p>
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
    border: solid;
    position: relative;
    font-family: Arial, Helvetica, sans-serif;
}
.usuario{
    //right: -17px;
    margin-top: 10px; 
    margin-left: 28px;
    display: flex;
    position: relative;
    align-items: center; 
    height: 100px;
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
    width: 100%;
    height: 50px;
    margin-top: 10px;
    color: $gris;
    &.mensaje-recibido{
        width: auto;
        height: auto ;
        font-size: 14px;
        border-radius: 6px;
        background: $degradado;
        color: $blanco;
        text-align: justify;
        max-width: 84%;  
        padding: 15px 15px 15px 15px;
    }
}
</style>


