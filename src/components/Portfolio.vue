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
                    "Project1",
                    "Project2",
                    "Project3",
                ],
                descr:[
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ut orci eu elit consequat posuere ut sed elit. Nulla et tristique felis. Morbi quis orci non purus blandit fringilla. Etiam et mollis eros. Duis venenatis vulputate lacus, non tristique eros placerat vel. Nam nec magna lacus. Etiam euismod egestas mauris nec mollis. Phasellus efficitur et ex vel condimentum. Cras enim purus, tempor sed massa vel, accumsan bibendum magna. Nullam hendrerit cursus purus, sit amet viverra arcu gravida vel.",
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ut orci eu elit consequat posuere ut sed elit. Nulla et tristique felis. Morbi quis orci non purus blandit fringilla. Etiam et mollis eros. Duis venenatis vulputate lacus, non tristique eros placerat vel. Nam nec magna lacus. Etiam euismod egestas mauris nec mollis. Phasellus efficitur et ex vel condimentum. Cras enim purus, tempor sed massa vel, accumsan bibendum magna. Nullam hendrerit cursus purus, sit amet viverra arcu gravida vel.",
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec ut orci eu elit consequat posuere ut sed elit. Nulla et tristique felis. Morbi quis orci non purus blandit fringilla. Etiam et mollis eros. Duis venenatis vulputate lacus, non tristique eros placerat vel. Nam nec magna lacus. Etiam euismod egestas mauris nec mollis. Phasellus efficitur et ex vel condimentum. Cras enim purus, tempor sed massa vel, accumsan bibendum magna. Nullam hendrerit cursus purus, sit amet viverra arcu gravida vel.",
                ]
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