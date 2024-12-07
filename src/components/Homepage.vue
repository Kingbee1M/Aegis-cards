<template>
    <div id="Home">
        <div class="wrapper">
            <div class="writting">
       <div class="Heading">The Print Business You Can Trust</div>
       <div class="content">We have a large range of products available, including serial and random numbering Scratch Cards, flyers, booklets, string labels, letterhead, and banners. For clients who do not have a design, we can provide design services.</div>
       <div class='minors'>
        <div class="scratch">Scratch Cards</div>
        <div class="others">Other paper products</div>
       </div>          
    </div>
       <div class="imageHolder"><img src="/images/Group 244.png"></div>
       </div>

    </div>
</template>

<script>
    export default {
        name: 'homePagee'
    }
</script>

<style scoped>
#Home {
    padding-top: 60px;
    padding-bottom: 10%;
    font-family: open sans;
    background-color: #EAF3FE;
    width: 100%;
    height: 100vh;
}

.wrapper {
    width: 100%;
    height: 70%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    margin-top: 10%;
}

.writting {
    width: 45%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: end;
    align-items: center;
    word-wrap: break-word;
    gap: 2%;
}


.Heading {
    font-size: 50px;
    font-weight: 700;
    line-height: 60px;
    width: 80%;
}

.content {
    font-weight: 400;
    font-size: 16px;
    width: 80%;
}

.imageHolder {
    height: 152.1%;
    width: 55.33%;
    display: flex;
    justify-content: end;
    align-items: center;
    /* width- 482px height-657px */
}

.imageHolder img {
    width: 90%;
    height: 90%;
}

.minors {
    width: 80%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.scratch {
    font-size: 18px;
    text-wrap: nowrap;
    background-color: #403BA2;
    padding: 5px 15px;
    border: 1px solid #403BA2;
    border-radius: 5px;
    color: white;

}

.others {
    text-wrap: nowrap;
    color: #5FBBDB;
    border: 2px solid #5FBBDB;
    border-radius: 5px;
    padding: 10px 10px;
}
</style>