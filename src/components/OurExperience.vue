<template>
    <div class="ourExperience">
        <div class="writting">
            <div>
            <div class="our">Our experience</div>
            <div class="you">You can <span class="purple">trust</span> us to serve you better</div>
            <div class="here">Here’s why</div>
            </div>
            <div class="cradDiv">
                <div class="purpleBorder item_1"></div>
                <div class="cards item_2">
                    <div class="head">9</div>
                    <div class="follow">Years of experience</div>
                </div>
                <div class="cards item_3">
                    <div class="head">20</div>
                    <div class="follow">
                        <div>Core</div>
                        <div>staffs</div>
                    </div>
                </div>
                <div class="cards item_4">
                    <div class="head">200+</div>
                    <div class="follow">Happy customers</div>
                </div>
            </div>
            <div class="contact">Contact us</div>
        </div>
        <div class="imageholder"><img src="/images/Our experience image.svg" alt="img5"></div>
    </div>
</template>

<script>
    export default {
        name: 'OurExperience'
    }
</script>

<style scoped>
.ourExperience {
    background: linear-gradient(to right, #4F4F4F 10%, #292929 90%);
    height: 720px;
    width: 100%;
    margin: 90px 0;
    color: #ffffff;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    font-family: open sans;
}

.writting {
    height: 80%;
    width: 40%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 50px;
}

.our {
    font-size: 20px;
    font-weight: 700;
    margin-left: 100px;
}

.you {
    font-size: 40px;
    word-wrap: break-word;
    width: 80%;
    font-weight: 700;
    font-family: inter;
    margin-left: 100px;
}

.here {
    font-size: 14px;
    font-weight: 400;
    margin-left: 100px;
}

.purple {
    color: rgb(186,183,255);
}

.cradDiv {
    width: 400px;    
    display: grid;
    justify-content: center;
    align-items: center;
    grid-template-rows: repeat(1, 90px);
    grid-template-columns: repeat(5, 90px);
}

.item_1 {
    grid-area: 1 / 1 / 1 / 2;
}
.item_2 {
    grid-area: 1 / 2 / 1 / 3;

}
.item_3 {
    grid-area: 1 / 3 / 1 / 4;
    margin-left: 30px
}
.item_4 {
    grid-area: 1 / 4 / 1 / 5;
    margin-left: 60px
}

.purpleBorder {
    width: 150px;
    height: 42px;
    background: linear-gradient(to right,  rgb(143,71,237, 1) 95%, rgb(143,71,237, 0) 5%);
    z-index: 1;
    opacity: 30%;
}
/* (186,183,255, 1) */

.cards {
    height: 90px;
    width: 95px;
    padding-left: 15px;
    background: linear-gradient(45deg, #F9F9F935, #FFFFFF15);
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: flex-start;
}

.head {
    font-size: 20px;
    font-family: inter;
    font-weight: 700;
}

.follow {
    font-size: 14px;
    font-family: inter;
    font-weight: 500;
}

.follow div{
    font-size: 14px;
    font-family: inter;
    font-weight: 500;
}

.contact{
    padding: 10px 35px;
    background-color: #BAB7FF;
    border-radius: 5px;
    margin-left: 100px;
}
</style>