<template>
    <div id="ContactUs">
        <div class="writting">
            <div class="first">
                <div class="see">See something you like?</div>
                <div class="conts"><img src="/images/Group 265.svg" alt="contact"></div>
                <div class="we">We’ll get back as soon as possible</div>
            </div>
            <div class="second">
                <form @submit.prevent="sendEmail">
                    <div><input type="text" placeholder="First Name - Last Name" v-model="formValues.name"></div>
                    <div><input type="tel" placeholder="Phone Number" v-model="formValues.number"></div>
                    <div><input type="email" placeholder="Email" v-model="formValues.email"></div>
                    <div><input type="time" placeholder="Time" v-model="formValues.time"></div>
                    <div><input type="date" placeholder="date" v-model="formValues.date"></div>
                    <div><textarea rows="10" cols="50" placeholder="Message" v-model="formValues.message"></textarea></div>
                    <button type="submit">Send an mail</button>
                </form>
             </div>
        </div>
        <div class="imageholder"><img src="/images/4322854 copy-01 1.svg"></div>
    </div>
</template>

<script>
import emailjs from 'emailjs-com';
    export default {
        data() {
            return{
                formValues : {
                    name: '',
                    number: '',
                    email: '',
                    message: '',
                    time: '',
                    date: ''
                }
            }
        },

        mounted() {
            emailjs.init('Hs7R-wekj7bSQ1NAz'); // Initialize EmailJS
        },
        methods: {
    async sendEmail() {
      try {
        const result = await emailjs.send(
          'service_szig23g',
          'Aegis_cards',
          this.formValues,
          's0JJW5QIFue_fjmzj'
        );
        console.log('Email sent successfully:', result.text);
        alert('Your message has been sent!');
      } catch (error) {
        console.error('Error sending email:', error);
        alert('Failed to send the message. Please try again.');
      }
    },
  },

    }
</script>

<style scoped>
#ContactUs {
    display:flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 100%;
}

.writting {
    width: 80%;
    margin-left: 100px;
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: flex-start;
    gap: 60px;
}

.first {
    font-family: open sans;
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: flex-start;
}

.see {
    color: #959595;
    font-weight: 700;
    font-size: 20px;
    margin-bottom: 10px;
}

.we {
    color: #4F4F4F;
    font-weight: 400;
    font-size: 16px;
}

input {
    width: 70%;
    margin-bottom: 20px;
    font-family: open sans;
    border-style: solid;
    border-width: thin;
    border-color: #B9B9B9;
    padding: 10px 60px
}

input:focus {
    width: 70%;
    margin-bottom: 20px;
    font-family: open sans;
    border-style: thin;
    border-width: 0 0 5px 0 ;
    outline: none;
}

button {
    color: white;
    font-family: open sans;
    margin-top: 30px;
    background-color: #403BA2;
    border: thin solid grey;
    padding: 10px 10px;
}
</style>