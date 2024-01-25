<template>
  <section class="header__content" id="#home">
    <div class="container">
        <div class="header__content-info">
            <p class="hello">Hello</p>
            <p class="name">I'M SHAHBOZ</p>
            <p class="header__content-descr">I've been doing web design, front-end and back-end development for a year now. Do you need a website design, site layout, or maybe a turnkey website? Then contact me</p>
            <button class="header__content-btn">CONTACT ME</button>
        </div>
        <div class="header__content-avatar">
            <div class="avatar-ellipse">
                <img src="../assets/images/ellipse.png" alt="">
            </div>
            <img src="../assets/images/avatar.png" alt="" class="avatar-img">
            <img src="../assets/images/avatar-head.png" alt="" class="avatar-head">
            <div class="avatar-item-ellipse item1">
                <span class="ellipse-component">UI</span>
            </div>
            <div class="avatar-item-ellipse item2">
                <span class="ellipse-component">&lt;/</span>
            </div>
            <div class="avatar-item-ellipse item3">
                <span class="ellipse-component">UX</span>
            </div>
            <div class="avatar-item-ellipse item4">
                <span class="ellipse-component">PS</span>
            </div>            
        </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scooped>
    .header__content{
        background: var(--bg1, linear-gradient(102deg, #2C2C2C 1.56%, #1C1C1C 95.55%));
        margin-top: -60px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        overflow: x;
    }
    .container{
        display: flex;
        justify-content: space-between;
    }
    .header__content-info{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        max-width: 447px;
        gap: 27px;
        margin-top: -80px;
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
    .avatar-ellipse{
        max-width: 675px;
        position: relative;
    }
    .avatar-img{
        position: absolute;
        bottom: -30px;
        right: 153px;
        object-fit: contain;
    }
    .avatar-head{
        position: absolute;
        top: 76px;
        right: 240px;
        transform: rotate(-6.566deg);
    }
    .ellipse-component{
        color: #00C4F0;
        font-family: NEXT-ART;
        font-size: 36px;
        font-weight: bold;
        line-height: normal;
    }
    .avatar-item-ellipse{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 90px;
        height: 90px;
        background: var(--Gray2, linear-gradient(131deg, #414141 0%, #2D2D2D 100.52%));
        border-radius: 50%;
    }
    .item1{
        position: absolute;
        top: 180px;
        right: 175px;
    }
    .item2{
        position: absolute;
        top: 250px;
        right: 600px;
    }
    .item3{
        position: absolute;
        top:425px;
        right: 640px;
    }
    .item4{
        position: absolute;
        top: 590px;
        right: 590px;
    }
</style>