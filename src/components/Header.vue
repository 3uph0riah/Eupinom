<template>
    <div class="header">
        <div class="button contact" @click="contact()">
            Contact
        </div>
        <div class="button telephone" @click="telephone()">
            Téléphone
        </div>
        <img class="photoCathy" src="../assets/img/cathy.jpg" alt="cathy"/>
    </div>
</template>

<script>

export default {
  name: "header",
  methods: {
    contact() {
        console.log("contact");
    },
    telephone() {
        window.open("tel:+33695661871", '_self');
    },
  },
};
</script>

<style scoped>
    .header {
        height: 35vh;
        background-color: #f37731;
        color: white;
        display: flex;
        flex-direction: column;
        text-align: center;
        justify-content: center;
        align-items: center;
        gap: 10px;   
    }

    .button {
        cursor: pointer;
        user-select: none;
        border: 1px solid white;
        padding: 5px;
        width: 15vw;        
    }

    .photoCathy {
        width: 8vw;
        border-radius: 50%;
    }
</style>