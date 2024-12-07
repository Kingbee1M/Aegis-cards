<template>
    <div id="AboutUs">
        <div class="All">All About us</div>
        <div class="wrapper">
            <div class="writting">
                <div class="act">
                    <div class="headings"><span class="blues">Born</span> in 2013</div>
                    <div class="content">Established in 2013 following the Management Buy Out of the scratch card plant belonging to CardCentre Nig. Ltd, a subsidiary of CHAMS PLC, by the previous Managing Director and his team of investors, AEGIS Cards Limited was formed. On the 4th of October, 2013, Aegis Cards Ltd gained physical control.</div>
                </div>
                <div class="act">
                    <div class="headings twin1">Dedicated to providing <span class="blues">quality service</span></div>
                    <div class="content">As one of the first set of NCC Licensed Scratch Card makers in Nigeria since 2005, we were a pioneer of prepaid voucher/scratch card manufacturers in Nigeria. We also offer "non-secure" paper products such as flyers, banners, and letterheads. </div>
                </div>
            </div>
            <div class="imageholder"><img src="/images/Image.png"></div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
#AboutUs {
    width: 100%;
    padding: 100px 0;
}

.All {
    color: #959595;
    font-weight: 700;
}

.wrapper {
    width: 100%;
    height: 80%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    gap: 30px;
}

.writting {
    width: 37%;
    height: 80%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 7%;
}

.act {
    width: 100%;
}

.headings{
    font-size: 40px;
    width: 100%;
    color: #000000;
    font-weight: 700;
    line-height: 48px;
    font-family: Inter;
}

.blues {
    color: rgb(95,187,219);
}

.content {
    height: 120px;
    width: 100%;
    font-size: 14px;
    overflow: hidden;
    word-wrap: break-word
}

.twin1 {
    height: 144px;
    width: 70%;
    min-width: 296px;
    margin-bottom: 3%;
}

.imageholder {
    height: 500px;
    width: 574px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.imageholder img {
    height: 544px;
    width: 574px;
}
</style>