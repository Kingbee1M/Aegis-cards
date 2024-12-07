<template>
        <div class="MainNavBar" ref="navbar" >
            <div class="sectionBar">
            <div><img src="/images/New Aegis Logo 1.png"></div>
            <div class="NavBar">
            <div><a href="#Home">Home</a></div>    
            <div><a href="#AboutUs" @click="scrolling">About Us</a></div>    
            <div><a href="#OurProduct">Our Products</a></div> 
            <div><a href="#ContactUs">Contact Us</a></div> 
            </div>
            </div>
            <div class="enquiry prioriize"><a href="#ContactUs">Send an enquiry</a></div>
        </div>
</template>

<script>
    export default {
        name: 'Navbar',
        data() {
            return {
        lastScrollY: 0, // Track the last scroll position
            }
        },
        methods: {
    handleScroll() {
      const currentScrollY = window.scrollY;

      // Access the navbar element using the ref
      const navbar = this.$refs.navbar;

      if (currentScrollY > 400) { // Threshold for hiding/showing the navbar
        if (currentScrollY > this.lastScrollY) {
          // Scrolling down - hide the navbar
          navbar.style.transform = "translateY(-100%)";
        } else {
          // Scrolling up - show the navbar
          navbar.style.transform = "translateY(0)";
        }
      } else {
        // At the top of the page - always show the navbar
        navbar.style.transform = "translateY(0)";
      }

      // Update lastScrollY
      this.lastScrollY = currentScrollY;
    },
  },
  mounted() {
    // Add scroll event listener when the component is mounted
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeUnmount() {
    // Clean up the event listener when the component is destroyed
    window.removeEventListener("scroll", this.handleScroll);
  },
    }
</script>

<style scoped>

.MainNavBar {
    background-color: #EAF3FE;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    position: fixed; /* Make it stick to the top */
    top: 0;
    left: 0;
    width: 100%;
    height: 50px;
    transition: transform 0.3s ease-in-out; /* Smooth transition for hiding */
    z-index: 1000;
}

.MainNavBar a {
    color: #292929;
    text-decoration: none;
    font-size: 1rem;
    word-wrap: break-word;
}

.MainNavBar a:hover {
    color: #403BA2;
    text-decoration: underline;
}

.MainNavBar a:active {
    color: #403BA2;
    text-decoration: underline;
}

.sectionBar {
    width: 60%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.NavBar {
    width: 50%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.enquiry {
    margin-right: 1%;
    background-color: #5FBBDB;
    padding: 10px 30px;
    border-radius: 15px; 
}

.MainNavBar .enquiry a:hover {
    color: white;
}

@media screen and (max-width: 760px) {
  .NavBar {
    width: 80%;
  }
  
  .MainNavBar {
    font-size: 10px;
  }
}
</style>