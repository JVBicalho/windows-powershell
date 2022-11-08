<script>
// Icons
import IconClose from  './icons/IconClose.vue'
import IconMaximize from  './icons/IconMaximize.vue'
import IconPowerShell from  './icons/IconPowerShell.vue'

export default {
    mounted() {
        this.$refs.input.focus();
    },
    components: { IconPowerShell }
}
</script>


<template>
  <div class="prompt">
    <div class="header">
        <div class="abas">
            <div class="aba">
                <span class="icon"><IconPowerShell/></span>Windows PowerShell<span class="icon"><IconClose /></span>
            </div>
            <div class="abas-icons">
                <span>plus</span>
                <span>arrow-down</span>
            </div>
        </div>
        <div class="icones">
            <span class="icon">-</span>
            <span class="icon">
                <IconMaximize  />
            </span>
            <span class="icon">
                <IconClose />
            </span>   
        </div>
    </div>
    <div class="alerta">
        <span class="icon">!</span>
        O Terminal do Windows pode ser definido como o aplicativo de terminal padrao em suas configuracoes. 
        <span class="open-conf"> Abrir Configuracoes</span>
        <span class="icon">
            <IconClose />
        </span>
    </div>
    <div class="input-area">
        O Windows PowerShell <br>
        Copyright (C) Microsoft Corporation. Todos os direitos reservados.<br>

        Instale o PowerShell mais recente para obter novos recursos e aprimoramentos! https://aka.ms/PSWindows <br>
        <br>
        <br>
        PS C:\Users\conta\Desktop>
    </div>
  </div>
</template>
<style scoped>
.prompt{
    background-color: black;
    color: #fff;
    
    border-radius: 0.5vw;
    border: 0.1vw solid #ccc;
    height: 33.4vw;
    display: flex;
    flex-direction: column;
   
    width: 59.5vw;
    
}
.icon{
    
    
}
.header{
    background-color: aqua;
    padding: 1vw ;
    
    border-radius: 0.1vw 0.1vw 0 0;
    height: 5vw;
    display: flex;
    flex-direction: row;

    
}
.alerta{
    padding: 2vw;
    background-color: rgb(46, 46, 46);
}
.open-conf{
    color: blue;
}
.input-area{
    font-family: "Cascadia Mono";
    
   
    color: #cCCCCC;
    padding: 1vw ;
}

</style>
