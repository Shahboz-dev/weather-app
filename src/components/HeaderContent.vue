<template>
  <section class="header__content" id="#home">
    <div class=" header__content-container container">
        <div class="header__content-info">
            <p class="hello">Hello</p>
            <p class="name">I'M SHAHBOZ</p>
            <p class="header__content-descr">I've been doing web design, front-end and back-end development for a year now. Do you need a website design, site layout, or maybe a turnkey website? Then contact me</p>
            <button class="header__content-btn">CONTACT ME</button>
        </div>
        <div class="avatar-img">
        </div>
         
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scooped>
    @media (max-width:991.99px){
        .hello{
            font-size: 30px !important;
        }
        .name{
            font-size:50px !important;
        }
        .header__content-btn{
            font-size: 12px !important;
            padding: 10px 25px !important;
        }
    }
    .avatar-img{
        background: url("../assets/images/avatar-img.png");
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        width: 500px;
        height: 400px;
        margin-bottom: 40px;
    }
    .header__content{
        background: var(--bg1, linear-gradient(102deg, #2C2C2C 1.56%, #1C1C1C 95.55%));
        overflow: x;
    }
    .header__content-info{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        max-width: 447px;
        gap: 27px;
    }
    .hello{
        color: var(--text, #E4E4E4);
        font-family: NEXT-ART;
        font-size: 40px;
        font-weight: 600;
    }
    .name{
        color: var(--text, #E4E4E4);
        font-family: NEXT-ART;
        font-size: 72px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
    .header__content-descr{
        color: var(--text, #E4E4E4);
        font-family: Arodora-Pro;
        font-size: 18px;
        font-style: normal;
    }
    .header__content-btn{
        border-style: none;
        border-radius: 6px;
        background: var(--orange, linear-gradient(87deg, #E2A300 4.47%, #E29500 95.53%));
        box-shadow: 0px 2px 13px 0px rgba(226, 158, 0, 0.48);
        color: #000;
        font-family: NEXT-ART;
        font-size: 18px;
        font-weight: 700;
        padding: 14px 38px;
    }
    .header__content-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>