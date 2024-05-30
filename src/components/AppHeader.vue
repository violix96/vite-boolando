<script setup>
</script>

<template>
 <header>
        <div class="container">
            <div class="row">
                <div class="col-25">
                    <ul>
                        <li><a href="">Donna</a></li>
                        <li><a href="">Uomo</a></li>
                        <li><a href="">Bambini</a></li>
                    </ul>
                </div>
                <div class="col-50">
                    <img class="logo" src="/img/boolean-logo.png" alt="Logo">
                </div>
                <div class="col-25">
                    <ul>
                        <li><a href=""><img class="logo-user" src="/img/user.png" alt="User"></a></li>
                        <li><a href=""><img class="logo-user" src="/img/like--v1.png" alt="Like"></a></li>
                        <li><a href=""><img  class="logo-user" src="/img/shopping-bag.png" alt="shopping-bag"></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </header>   
</template>

<style scoped lang="scss">
header{
    position: fixed;
    padding: 15px 0px;
    background-color: orangered;
    width: 100%;
    z-index: 1;
  
}

.col-25{
    width: 25%;
    /* height: 40px;
    border: 1px solid black; */
    padding: 8px 0px;
}

.row{
    display: flex;
    flex-wrap: wrap;
}
</style>
