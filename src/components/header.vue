<script setup>
defineProps({
    nama: {
        type: String,
        default: "Agus Salimu",
    },
    role: {
        type: String,
        default: "Web Desainer",
    },

});
</script>
<template>
        <section class="header">
            <img src="../assets/profile-1.png" alt="" height="250">
            <div class="header__container">
                <h1>{{ nama}}</h1>
                <h3>{{ role }}</h3>
                <div class="header__btn">
                    <button>Download CV</button>
                    <button>Chat Me</button>
                </div>
            </div>
        </section>
</template>