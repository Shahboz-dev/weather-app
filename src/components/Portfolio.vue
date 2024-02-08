<template>
  <section id="portfolio" class="portfolio">
    <h1 class="portfolio__header">PORTFOLIO</h1>
    <div class="portfolio__content container">
        <div class="portfolio__content-slider">
            <button class="portfolio-btn" @click="swapLeft" >
                <img src="../assets/images/button-arrow-left.png" alt="">
            </button>
            <Project 
                :i="i"
                :data="data"
                :count="count"
                :active="active"
            />
            <button class="portfolio-btn" @click="swapToRight">
                <img src="../assets/images/button-arrow-right.png" alt="">
            </button>
        </div>
    </div>
  </section>
</template>

<script>
import Project from "../components/Project.vue"
export default {
    components:{
        Project
    },
    data(){
        return {
            i:0,
            count:0,
            Active:1,
            data:{
                header: [
                    "VUE Weather",
                    "Burgers",
                    "NurEdu",
                ],
                descr:[
                    "This application was developed when I only started my journey into VUE. It uses weather API to get the data about all the regions on the Earth, so you can litteraly know the weather forecast for any territory on the planet. You can search the territory using search bar on the top right corner of the page and by pressing ENTER , you can see the weekly forecast for that region",
                    "Project Burgers was developed using Angular. It fetches different types of burgers using the Burgers-API. You can easily navigate through the web page and dynamicly change the currency. Finally you can order a burger in the footer where all the form validation has been added.",
                    "NurEdu is a special platform for learners that want to know more about online school NurEducation. In the application I used Flask to develop the backend and also used SQLite3 to store data. You as a user can leave your credentials in the form that will be dynamicly stored in the database",
                ],
            }
        }
    },
    methods:{
        swapToRight(){
            if (this.i == (this.data.header.length)-1){
                this.i = 0;
            }else{
                this.i++;
            }
        },
        swapLeft(){
            if(this.i == 0){
                this.i = (this.data.header.length)-1
            }else{
                this.i--;
            }
        }
    }
}
</script>

<style>
    @media (max-width:1199.99px) {
        .portfolio-btn{
            width: 50px !important;
            height: 50px !important;
        }
    }
    @media (max-width:991.99px) {
        .portfolio__content-slider{
            flex-direction: column;
        }
    }
    .portfolio__content{
        padding-bottom: 150px;
    }
    .portfolio{
        background: linear-gradient(101.56deg, #2C2C2C 1.56%, #1C1C1C 95.55%);
    }
    .portfolio__content-slider{
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 30px;
    }
    .portfolio__header{
        font-family: NEXT ART;
        font-size: 48px;
        font-weight: 400;
        line-height: 54px;
        letter-spacing: 0em;
        color:white;
        text-align: center;
        padding: 100px 50px;
    }
    .portfolio-btn{
        width: 60px;
        height: 60px;
        border-style: none;
        border-radius: 50%;
        background: orange;
        
    }
    .portfolio-btn :hover{
        cursor: pointer;
    }
</style>