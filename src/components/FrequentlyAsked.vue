<template>
    <div id='frequent'>
        <div class="wrapper">
            <div class="first">Frequently asked questions</div>
            <div class="second">
                <div class="imageholder"><img src="/images/FAQ illustrator.svg" alt="FAQ ILLUSTRATOR"></div>
                <div class="writting">
                    <div class="section">
                        <div class="tabs"><div class="QandA">How long would it take to print?</div><div class="answer" v-show="isVisible1">This depends on your order quantity and any specific requirements you have. Typically we take a minimum of 2 days to print and get it ready for delivery</div></div>
                        <div><button @click="quickAns1()" v-show="isBtnvisible1" class="btn"><img src="/images/Group 218.png" alt="add sign"></button><button @click="quickAns1()" v-show="isVisible1"class="btn2"><img src="/images/Group 218 (1).png" alt="add sign"></button></div>
                    </div>
                    <div class="section">
                        <div class="tabs"><div class="QandA">How long does it take to recieve my order?</div><div class="answer" v-show="isVisible2">After the printing and Quality control has been concluded, it will be deliverd to you the next day
                        </div></div>
                        <div><button @click="quickAns2()" v-show="isBtnvisible2" class="btn"><img src="/images/Group 218.svg" alt="add sign"></button><button @click="quickAns2()" v-show="isVisible2"class="btn2"><img src="/images/Group 218 (1).png" alt="add sign"></button></div>
                    </div>
                    <div class="section">
                        <div class="tabs"><div class="QandA">How is the payment concluded</div><div class="answer" v-show="isVisible3">Payment can be made through diffrent ways, feel free to contanct us to get a price range and payment option</div></div>
                        <div><button @click="quickAns3()" v-show="isBtnvisible3" class="btn"><img src="/images/Group 218.svg" alt="add sign"></button><button @click="quickAns3()" v-show="isVisible3"class="btn2"><img src="/images/Group 218 (1).png" alt="add sign"></button></div>
                    </div>
                    <div class="section">
                        <div class="tabs"><div class="QandA">What types of products do you produce?</div><div class="answer" v-show="isVisible4">We crate all types of cards and paper designs</div></div>
                        <div><button @click="quickAns4()" v-show="isBtnvisible4" class="btn"><img src="/images/Group 218.svg" alt="add sign"></button><button @click="quickAns4()" v-show="isVisible4"class="btn2"><img src="/images/Group 218 (1).png" alt="add sign"></button></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'frequent',
        data() {
            return {
                isBtnvisible1: true,
                isBtnvisible2: true,
                isBtnvisible3: true,
                isBtnvisible4: true,
                isVisible1: false,
                isVisible2: false,
                isVisible3: false,
                isVisible4: false,
            }
        },
    

        methods: {
            quickAns1() {
                this.isBtnvisible1 = !this.isBtnvisible1
                this.isVisible1 = !this.isVisible1
            },

            quickAns2() {
                this.isBtnvisible2 = !this.isBtnvisible2
                this.isVisible2 = !this.isVisible2
            },

            quickAns3() {
                this.isBtnvisible3 = !this.isBtnvisible3
                this.isVisible3 = !this.isVisible3
            },

            quickAns4() {
                this.isBtnvisible4 = !this.isBtnvisible4
                this.isVisible4 = !this.isVisible4
            },



        }

}
</script>

<style scoped>
#frequent {
    background: linear-gradient(to right, #4F4F4F 20%, #292929 80%);
    width: 100%;
    height: 568px;
    margin-top: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.wrapper {
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: flex-start;
    gap: 50px;
}

.first {
    color: white;
    font-weight: 700;
    font-family: Open Sans;
    margin-left: 20px;
}

.second {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: flex-start;
}

.writting {
    font-family: open sans;
    font-size: 14px;
    font-weight: 400;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 60px;
    width: 60%;
}

.tabs {
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: flex-start;
    color: #4F4F4F;
    width: 65%;
    height: 50px;
    background-color: white
}

.section {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: flex-start;
    width: 100%;
}

button {
    all: unset; /* Removes all default styles */
    display: inline-block; /* Makes the button behave like an inline element */
     padding: 0; /* Removes padding */
     border: none; /* Removes border */
     background: none; /* Removes background */
     cursor: pointer; /* Ensures it behaves like a clickable button */
     margin-left: 10px;
     height: 70%;
}
.btn {
    height: 100%;
}

.btn2 {
    all: unset; /* Removes all default styles */
    display: inline-block; /* Makes the button behave like an inline element */
     padding: 0; /* Removes padding */
     border: none; /* Removes border */
     background: none; /* Removes background */
     cursor: pointer; /* Ensures it behaves like a clickable button */
     margin-left: 10px;
     height: 90px;
}

.btn2 img {
    height: 100%;
}

.QandA {
    width: 100%;
    height: 100%;
    padding: 14px 0px;
    font-size: 14px;
    font-weight: 600;
    padding-left: 10px;
    background-color: white


}

.answer {  
    width: 100%;
    height: 70px;
    font-size: 12px;
    font-weight: 400;
    padding-left: 10px;
    padding-bottom: 10px;
    background-color: white
}

</style>