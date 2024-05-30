<script>
export default {
    data() {
        return {
            cards: [
                {
                    name: 'RELAXED',
                    brand: "Levi's"
                }
            ]
        }
    }
}
</script>

<template>
<div class="container">
    <div class="row">
        <div class="col-33" v-for="card in cards">
            <div class="content">
                <div>
                    <img class="main-img" src="./img/1.webp" alt="Prodotto 1">
                    <img class="hover-img" src="./img/1b.webp" alt="Prodotto1b">
                    <div class="absolute">
                        <span class=" sconti-label">50%</span>
                        <span class="sostenibilità-label">Sostenibilità</span>
                    </div>
                    <div class="content-like">
                        <span class="cuoricino"> &#10084;</span>
                        <span class="cuoricino-hover"> &#10084;</span>
                    </div>
                    <p>Levi's</p>
                    <h4>RELAXED FIT TEE UNISEX</h4>
                    <span class="prezzo-ora">14.99 &#8364;</span>
                    <span class="prezzo-prima">29.99 &#8364;</span>
                </div>
            </div>
        </div>
    </div>
</div>
</template>