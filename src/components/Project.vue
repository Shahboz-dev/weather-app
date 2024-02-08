<template>
        <div class="slider__content">
            <img src="../assets/images/project1.jpg" alt="product" class="project-img" v-if="data.header[i] == 'VUE Weather'">
            <img src="../assets/images/project2.jpg" alt="product" class="project-img" v-if="data.header[i] == 'Burgers'">
            <img src="../assets/images/project3.jpg" alt="product" class="project-img" v-if="data.header[i] == 'NurEdu'">
            <div class="project__content-info">
                <h3 class="project-info-header">{{data.header[i]}}</h3>
                <p class="project-info-text">{{data.descr[i]}}</p>
                <a href="https://github.com/Shahboz-dev/weather-app-2.git" class="project-info-demo" v-if="data.header[i] == 'VUE Weather'">SEE CODE</a>
                <a href="https://github.com/Shahboz-dev/burgers.git" class="project-info-demo" v-if="data.header[i] == 'Burgers'">SEE CODE</a>
                <a href="https://github.com/Shahboz-dev/NurEdu.git" class="project-info-demo" v-if="data.header[i] == 'NurEdu'">SEE CODE</a>
            </div>
        </div>
</template>

<script>
export default {
    name:"Project",
    props:{
        data:Object,
        i:Number,
        count:Number,   
    }
}
</script>

<style>
    @media (max-width:1199.99px) {
        .project-img{
            width: 350px !important;
            height: 350px !important;
        }
        .project-info-text{
            font-size: 14px !important;
        }
        .project-info-header{
            font-size: 20px !important;
        }
        .slider__content{
            padding: 30px !important;
        }
    }
    .project-info-text{
        font-family: Arodora Pro;
        font-size: 18px;
        font-weight: 300;
        line-height: 21px;
        letter-spacing: 0em;
        text-align: center;
        max-width: 300px;
    }
    .slider__content{
        display: flex;
        gap: 100px;
        padding: 50px;
        background: linear-gradient(130.68deg, #414141 0%, #2D2D2D 100.52%);
        border-radius: 29px;
    }
        .project-info-header{
        font-family: Arodora Pro;
        font-size: 24px;
        font-weight: 300;
        line-height: 29px;
        text-align: center;
        color: white;
        max-width: 250px;
    }
    .project__content-info{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items:center;
        gap: 25px;

    }
    .project-img{
        border-radius: 30px;
        width:500px;
        height: 500px;
        object-position: left;
        object-fit: cover;
    }
    .project-info-demo{
        color: orange;
    }
</style>