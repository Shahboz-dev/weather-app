<template>
  <footer id="contact" class="footer__content">
    <div class="container content">
        <div class="footer__content-info">
            <p class="p">Email: nuriddinovshaxboz1507@gmail.com</p>
            <p class="p">Inst: nastalgy.e.e</p>
            <p class="p">Calls: +998902521507</p>
        </div>
        <div class="footer__content-copyright">
            <img src="../assets/images/ui.svg" alt="">
            <p class="p">Copyright 2021, Notitanic</p>
        </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scooped>
    p{
        font-family: Arodora Pro;
        font-size: 18px;
        font-weight: 300;
        line-height: 21px;
        letter-spacing: 0em;
        color: white;
    }
    .footer__content{
        background: linear-gradient(130.68deg, #414141 0%, #2D2D2D 100.52%);
        padding: 50px;
    }
    .content{
        display: flex;
        justify-content: center;
        gap: 200px;
    }
    .footer__content-info{
        display: flex;
        flex-direction: column;
        gap: 18px;
    }
    .footer__content-copyright{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 20px;
    }
</style>