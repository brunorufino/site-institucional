<template>
   <main>

        <div class="text-top"> Vídeos novos toda <b> quinta </b>  ás <b> 20h </b></div>
          <a href="#" target=" blank">
            <img alt="Inscreva-se" id="subscribe" src="https://raw.githubusercontent.com/william-costa/wdev-mock-site-resources/master/assets/images/subscribe.svg">
        </a>
        <div class="text-button">youtube.com.br</div>
   </main>
</template>

<script>
export default {
    name: 'Home'
}
</script>

<style scoped>
 .text-top{
      color: var(--color-text-light);
      font-size: 22px;
      margin-bottom: 15px;
 }
 .text-button{
     color: var(--color-text-light);
     font-size: 18px;
     margin-top: 15px;
 }
 #subscribe{
     width: 340px;
 }
 main{
     background-color: var(--color-background-home);
     justify-content: center;
     align-items: center;
 }

 @media (min-width: 700px){
      #subscribe{
     width: 370px;
 }
 }
</style>