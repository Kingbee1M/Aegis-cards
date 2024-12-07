<template>
    <div id="OurProduct">
        <div class="what">What we do</div>
        <div class="create">Creating <span class="blues">magic</span class="blues"> with paper</div>
            <div class="holder">
        <div class="container">
            <div class="group1">
            <div class="item"><img src="/images/Group 190.svg"></div>
            <div class="item"><img src="/images/Group 190.png"></div>
            </div>
            <div class="group2">
            <div class="item"><img src="/images/Rectangle 112.png"></div>
            <div class="item"><img src="/images/Rectangle 112 (1).png"></div>
            <div class="item"><img src="/images/Rectangle 112 (2).png"></div>
            </div>
        </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ourproducts',
    }
</script>

<style scoped>
#OurProduct {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 20px;
}

.what {
    font-weight: 700;
    font-size: 20px;
    color: #959595;
}

.create {
    width: 368px;
    height: 96px;
    font-family: Inter;
    font-weight: 700;
    font-size: 40px;
    line-height: 48px;
    margin-bottom: 20px;
}

.holder {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    gap: 30px;
    width: 100%;
}

.group1 {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.group2 {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.item {
    width: 100%;
}

/* .container {
    display: grid;
    grid-template-columns: repeat(8, 12.5%);
    grid-template-rows: repeat(2, 272.89px);
    grid-gap: 20px 10px;
}

.blues {
    color: rgb(95,187,219);
}

.item_1 {
    grid-area: 1 / 1 / 1 / 5;
    overflow: hidden;

}

.item_2 {
    grid-area: 1 / 5 / 1 / 9;
    overflow: hidden;
}


.item_3 {
    grid-area: 2 / 1 / 2 / 3;
    overflow: hidden;
    
}

.item_4 {
    grid-area: 2 / 4 / 2 / 6;
    overflow: hidden;
}

.item_5 {
    grid-area: 2/ 7 / 2 / 9;
    overflow: hidden;
} */


</style>