<script>
// Icons
import IconPowerShell from  './icons/IconPowerShell.vue'
import IconMaximize from  './icons/IconMaximize.vue'
import IconClose from  './icons/IconClose.vue'

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
                <span><IconPowerShell/></span>Windows PowerShell<span>close</span>
            </div>
            <div class="abas-icons">
                <span>plus</span>
                <span>arrow-down</span>
            </div>
        </div>
        <div class="icones">
            <span>-</span>
            <span>
                <IconMaximize/>
            </span>
            <span>
                <IconClose/>
            </span>   
        </div>
    </div>
    <div class="alerta">
        <span>!</span>
        O Terminal do Windows pode ser definido como o aplicativo de terminal padrao em suas configuracoes. <span> Abrir Configuracoes</span>
        <span>close</span>
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
    border: 0.1vw;


    
}
.header{
    background-color: aqua;
    padding: 1vw ;
    display: flex;
    flex-direction: row;

}
.alerta{
    padding: 2vw;
}
.input-area{
    font-family: "Cascadia Mono";
    color: #CCCCCC;
    padding: 1vw ;
}

</style>
