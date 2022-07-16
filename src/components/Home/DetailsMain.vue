<template>
  <div class="details-container">
    <div class="wrapper">
      <i class='bx bx-server'></i>
      <span>80+</span>
      <h2>Servidores</h2>
      <p>Onde quer que a festa esteja!</p>
    </div>
    <div class="wrapper">
      <i class='bx bx-server'></i>
      <span>200k+</span>
      <h2>Usuários</h2>
      <p>Ouvindo o que tem de melhor.</p>
    </div>
    <div class="wrapper">
      <i class='bx bx-server'></i>
      <span>20+</span>
      <h2>Comandos</h2>
      <p>Logo mais aprende a cozinhar.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "DetailsMain",
};
</script>

<style lang="scss" scoped>
.details-container{
  display:grid;
  width: 70%;
  margin: 15em auto 23em ;
  grid-template-columns: repeat(3, 1fr);
  gap: 10em;
  .wrapper{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1em;
    text-align: center;
    .bx-server{
      border-radius: 50px;
      border: 1px solid var(--c-blue);
      padding: .5em;
      font-size: 2em;
      color: var(--c-blue);
    }
    span{
      color: var(--c-orange);
      font-weight: 700;
      font-size: 1.5em;
    }
    h2{
      font-size: var(--fsize-md);
    }
  }
  .wrapper:nth-child(1), .wrapper:nth-child(2){
    position: relative;
    &::before{
      content: '';
      position: absolute;
      width: 50%;
      height: 1px;
      background-color: var(--c-black);
      right: -50%;
      top:15%;
    }
  }
}
</style>