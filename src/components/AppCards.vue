<script>
export default {
    data() {
        return {
            cards: [
                {
                    name: 'RELAXED FIT TEE UNISEX',
                    brand: "Levi's",
                    prezzoA: "14.99 €",
                    prezzoP: "29.99 €",
                    img: "./img/1.webp",
                    imgH: "./img/1b.webp",
                    sconto: "50%",
                    sos: " Sostenibilità"
                }, 
                {
                    name: 'ROSES TEE',
                    brand: "Guess",
                    prezzoA: "20.99 €",
                    prezzoP: "29.99 €",
                    img: "./img/2.webp",
                    imgH: "./img/2b.webp",
                    sconto: "30%",
                    sos: " "
                }, 
                {
                    name: "Come zucchero filato",
                    brand: "Levi's",
                    prezzoA: "129.99 €",
                    prezzoP: "29.99 €",
                    img: "./img/3.webp",
                    imgH: "./img/3b.webp",
                    sconto: "30%",
                    sos: ""
                }, 
                {
                    name: 'TEE UNISEX',
                    brand: "Levi's",
                    prezzoA: "14.99 €",
                    prezzoP: "29.99 €",
                    img: "./img/4.webp",
                    imgH: "./img/4b.webp",
                    sconto: "50%",
                    sos: " Sostenibilità"
                }, 
                {
                    name: 'STRIPE BODICE',
                    brand: "Maya Deluxe",
                    prezzoA: "99.99 €",
                    prezzoP: "",
                    img: "./img/5.webp",
                    imgH: "./img/5b.webp",
                }, 
                {
                    name: 'MAGLIONE - BLACK',
                    brand: "Espirit",
                    prezzoA: "20.99 €",
                    prezzoP: "",
                    img: "./img/6.webp",
                    imgH: "./img/6b.webp",
                    sconto: "",
                    sos: " Sostenibilità"
                }, 


            ]
        }
    }
}
</script>

<template>
<div class="container" >
    <div class="row" >
        <div class="col-33" v-for="card in cards">
            <div class="content">
                <div>
                    <img class="main-img" :src="card.img" alt="Prodotto 1">
                    <img class="hover-img" :src="card.imgH" alt="Prodotto1b">
                    <div class="absolute">
                        <span class=" sconti-label" v-if="card.sconto!==''">{{ card.sconto }}</span>
                        <span class="sostenibilità-label">{{ card.sos }}</span>
                    </div>
                    <div class="content-like">
                        <span class="cuoricino"> &#10084;</span>
                        <span class="cuoricino-hover"> &#10084;</span>
                    </div>
                    <p>{{ card.brand }}</p>
                    <h4>{{card.name}}</h4>
                    <span class="prezzo-ora">{{ card.prezzoA }}</span>
                    <span class="prezzo-prima">{{ card.prezzoP}}</span>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped lang="scss">
.container{
    padding-top: 100px;
}

.sostenibilità-label{
    width: 100px;
    text-align: center;
    color: white;
    background-color: green;
    display: inline-block;
    bottom: 500px;
    left: 100px;
}

.absolute{
   
    bottom: 100px;
    left: 0px;
}

.prezzo-prima{
    padding-left: 10px;
}
</style>