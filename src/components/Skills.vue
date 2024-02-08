<template>
  <section class="skills__content">
    <div class="container">
        <ul class="skills__content-list">
            <li class="skills__content-list-item">
                <img src="../assets/images/pr-design.svg" alt="" class="list-item-img">
                <p class="list-item-text">Product Design</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/UI-UX.png" alt="" class="list-item-img">
                <p class="list-item-text">UX/UI Design</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/icon-design.svg" alt="" class="list-item-img">
                <p class="list-item-text">Icon Design</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/logo-design.svg" alt="" class="list-item-img">
                <p class="list-item-text">Logo Design</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/backend.svg" alt="" class="list-item-img">
                <p class="list-item-text">Backend</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/frontend.svg" alt="" class="list-item-img">
                <p class="list-item-text">Frontend</p>
            </li>
            <li class="skills__content-list-item">
                <img src="../assets/images/motion.svg" alt="" class="list-item-img">
                <p class="list-item-text">Motion</p>
            </li>
        </ul>
    </div>
    <About/>
  </section>
</template>

<script>
import About from "../components/About.vue"
export default {
    components:{
        About
    }
}
</script>

<style scooped>
    .skills__content{
        padding: 113px 100px;
        background: var(--Gray2, linear-gradient(131deg, #414141 0%, #2D2D2D 100.52%));
    }
    .skills__content-list{
        display: flex;
        justify-content: center;
        gap: 30px;
        flex-wrap: wrap;
    }
    .skills__content-list-item{
        width: 270px;
        height: 270px;
        border-radius: 29px;
        background: #2A2A2A;
        box-shadow: 0px 4px 6px 0px rgba(0, 0, 0, 0.47);
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 60px;
        align-items: center;
    }
    .list-item-text{
        color: var(--text, #E4E4E4);
        font-family: Arodora-Pro;
        font-size: 24px;
        font-style: normal;
        font-weight: 300;
        line-height: normal;
    }
    .skills__content-list-item:nth-child(1){
        gap: 20px;
    }
    .skills__content-list-item:nth-child(2){
        gap: 70px;
    }
</style>