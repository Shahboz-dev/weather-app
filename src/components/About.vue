<template>
  <section id="about" class="about__content">
    <div class="about__content-main container">
        <div class="about">
            <h1 class="about__content-title">ABOUT ME</h1>
            <p class="about__content-text">
                Hello again everyone! So, you already know that my name is Shahboz. A little about myself: student of Presidential School in Gulistan,Uzbekistan, 17 y.o., I love creativity since childhood, I live in Syrdarya, Uzbekistan. Why programming? Everything is elementary - I like it, the profession of the future, thanks to which I can provide myself and fulfill my dream - travel, at the moment I specialize in web design, front-end and back-end development, turnkey websites. Why should you choose me? I approach each order with great responsibility and love, as I want to make a name for myself, exclude plagiarism and negligence, fully study the project, the client and its target audience, work for quality, trying to make an order as quickly and uniquely as possible, taking into account all the edits and wishes.
                By trusting me, you will get the maximum return for your project, save your nerves and time.
                If you are interested in me , you want to know something more or use my services, then I will provide all my contacts below
            </p>
            <img src="../assets/images/about-img2.jpg" alt="" class="about-img1">
            <img src="../assets/images/about-img1.jpg" alt="" class="about-img2">
            <img src="../assets/images/about-img3.jpg" alt="" class="about-img3">
        </div>
        
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scooped>
@media (max-width:1199.99px) {
    .about-img2{
        max-width: 250px !important;
        right: -45% !important;
    }
    .about-img1{
        padding: 14px !important;
        max-width: 260px !important;
        object-position: center;
        object-fit: contain;
    }
}
@media (max-width:991.99px) {
    .about-img2{
        right: -45% !important;
        padding: 20px !important;
        max-width: 200px !important;
    }
    .about-img1{
        max-width: 220px !important;
        left: -50% !important;
        padding: 10px !important;
    }
    .about-img3{
        max-width: 220px !important;
        padding: 20px !important;
    }
   .about__content-text{
    padding: 40px !important;
    font-size: 12px;
    max-width: 370px !important;
   } 
}
    .about{
        position: relative;
    }
    .about__content{
        padding-top: 150px;
    }
    .about__content-main{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 36px;
    }
    .about__content-title{
        color: white;
        font-family: NEXT-ART;
        font-size: 48px;
        font-weight: 400;
        position: absolute;
        top: -25px;
        left: 20%;
        z-index: 2;
    }
    .about__content-text{
        font-family: Arodora-Pro;
        font-size: 16px;
        font-weight: 300;
        line-height: 24px;
        letter-spacing: 0.01em;
        color: white;
        max-width: 450px;
        padding: 63px;
        background: #2C2C2C;
        border-radius: 14px;
        z-index: 1;
    }
    .about-img1{
        max-width: 272px;
        min-height: 280px;
        object-position: center;
        position: absolute;
        top: 20px;
        left: -240px;
        padding: 30px;
        background: #2C2C2C;
        border-radius: 14px;
        z-index: 1;
    }
    .about-img2{
        background: #2C2C2C;
        border-radius: 14px;
        max-width: 300px;
        position: absolute;
        padding: 30px;
        top: 20%;
        right: -55%;
        z-index: 1;
    }
    .about-img3{
        background: #2C2C2C;
        border-radius: 14px;
        max-width: 272px;
        position: absolute;
        padding: 30px;
        bottom: -30px;
        left: -50%;
        z-index: 1;
    }
</style>