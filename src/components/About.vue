<template>
  <section id="about" class="about__content">
    <div class="about__content-main container">
        <h1 class="about__content-title">ABOUT ME</h1>
        <p class="about__content-text">Hello again everyone! So, you already know that my name is Shahboz. A little about myself: student of Presidential School in Gulistan,Uzbekistan, 17 y.o., I love creativity since childhood, I live in Syrdarya, Uzbekistan. Why programming? Everything is elementary - I like it, the profession of the future, thanks to which I can provide myself and fulfill my dream - travel, at the moment I specialize in web design, front-end and back-end development, turnkey websites. Why should you choose me? I approach each order with great responsibility and love, as I want to make a name for myself, exclude plagiarism and negligence, fully study the project, the client and its target audience, work for quality, trying to make an order as quickly and uniquely as possible, taking into account all the edits and wishes.
By trusting me, you will get the maximum return for your project, save your nerves and time.
If you are interested in me , you want to know something more or use my services, then I will provide all my contacts below.</p>
        <img src="../assets/images/about-img1.png" alt="" class="about-img1">
        <img src="../assets/images/about-img2.png" alt="" class="about-img2">
        <img src="../assets/images/about-img3.png" alt="" class="about-img3">
        <img src="../assets/images/White-ellipse.png" alt="" class="white-ellipse">
        <img src="../assets/images/yellow-ellipse.png" alt="" class="yellow-ellipse">
        <img src="../assets/images/blue-ellipse.png" alt="" class="blue-ellipse">
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scooped>
    .about__content{
        padding-top: 150px;
        position: relative;
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
        top: 125px;
        left: 40%;
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
        position: absolute;
        top: 130px;
        left: 200px;
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
        top: 300px;
        right: 200px;
        z-index: 1;
    }
    .about-img3{
        background: #2C2C2C;
        border-radius: 14px;
        max-width: 272px;
        position: absolute;
        padding: 30px;
        bottom: -20px;
        left: 200px;
        z-index: 1;
    }
    .white-ellipse{
        position: absolute;
        max-width: 780px;
        top: 130px;
        left: 0;
    }
    .yellow-ellipse{
        position: absolute;
        max-width: 356px;
        top: 70px;
        right: 220px;

    }
    .blue-ellipse{
        position: absolute;
        bottom: -100px;
        right: 200px;
        max-width: 486px;
    }
</style>