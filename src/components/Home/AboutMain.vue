<template>
<section class="about">
    <div class="about-container">
    <img src="@/assets/about-bg.png" alt="" class="about-bg">

        <h3>
            <span>Músicas de qualidade?</span>
            <span>Conheça o <span class="brand">Flame Play</span></span>
        </h3>
        <p>Flame Play é um bot de música com a finalidade de trazer a melhor proposta de Bot de música para seu servidor do discord. Praticidade e qualidade em um produto só!</p>
        <div class="player-wrapper">
            <p>Encontre suas faixas favoritas <i class='bx bx-search'></i></p>
            <img src="@/assets/musicplayer-1.png" alt="">
            <img src="@/assets/musicplayer-2.png" alt="">
            <img src="@/assets/musicplayer-3.png" alt="">

        </div>
        <h3>Em fest com mais de 200 mil pessoas, querendo festejar com você também!</h3>
    </div>
</section>

</template>

<script>
export default {
  name: "AboutMain",
};
</script>

<style lang="scss" scoped>
.about{
    position: relative;
}
.about-bg{
    width: 100%;    
    position: absolute;
    top: -30%;
}
.about-container{
    padding-top: 3em;
    background-color: var(--c-blue);
    position: relative;
    color: var(--c-white);
    display: flex;
    flex-direction: column;
    align-items: center;
    h3{
        font-size: var(--fsize-lg);
    }
    h3:nth-child(2){
        display: flex;
        flex-direction: column;
        line-height: 45px;
        .brand{
            color: var(--c-orange);
            font-family: var(--f-brand);
        }
    }
}
</style>