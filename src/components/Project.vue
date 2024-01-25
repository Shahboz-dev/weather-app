<template>
        <div class="slider__content">
            <img src="../assets/images/project1.png" alt="product" class="project-img" v-if="data.header[i] == 'Project1'">
            <img src="../assets/images/project2.png" alt="product" class="project-img" v-if="data.header[i] == 'Project2'">
            <img src="../assets/images/project3.png" alt="product" class="project-img" v-if="data.header[i] == 'Project3'">
            <div class="project__content-info">
                <h3 class="project-info-header">{{data.header[i]}}</h3>
                <p class="project-info-text">{{data.descr[i]}}</p>
                <a href="" class="project-info-demo">View demo</a>
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
        max-width:500px;
    }
    .project-info-demo{
        color: orange;
    }
</style>