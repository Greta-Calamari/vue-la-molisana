<template>
    <div class="prod-card">
        <img :src="detail.src" :alt="detail.titolo">
        <h3>{{detail.titolo}}</h3>
    </div>
</template>


<script>
export default {
    name: 'ProductCard',
    data(){
        return {
            links: [
                {
                    text: "Home",
                    url: "#",
                    active: false,
                },
                {
                    text: "Prodotti",
                    url: "#",
                    active: true,
                },
                {
                    text: "Chi Siamo",
                    url: "#",
                    active: false,
                },
                {
                    text: "Contatti",
                    url: "#",
                    active: false,
                },
            ],
        }
    },
    props: {
        detail: Object
        // immagine: String,
        // titolo: String
    }
    //['immagine','titolo']
}
</script>
<style lang="scss" scoped>
@import "../style/vars";
.prod-card {
	flex-basis: 25%;
	padding: 20px;
	background-color: white;
	border: 2px solid lighten($primary, 70%);
	h3 {
		color: $primary;
	}
	img {
		display: block;
	}
}
</style>