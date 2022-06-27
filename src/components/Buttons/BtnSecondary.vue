<template>
  <button class="btn-secondary">
    {{ btnAction }}
  </button>
</template>

<script>
export default {
  name: "BtnSecondary",
  props: {
    btnAction: String,
  },
};
</script>

<style lang="scss">
.btn-secondary {
  background-color: transparent;
  border: 1px solid var(--c-black);
  border-radius: 0.3em;
  color: var(--c-black);
  display: flex;
  align-items: center;
  padding: 0.6em 1.2em;
  font-weight: var(--fweight-b);
  cursor: pointer;
  transition: 0.4s ease;
  span {
    margin-left: 0.5em;
  }
  &:hover {
    color: var(--c-white);
    background-color: var(--c-black);
    box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 15px -3px,
      rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;
    transition: 0.4s ease;
  }
}
</style>
