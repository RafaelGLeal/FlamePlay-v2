<template>
  <button class="btn-primary">
    {{ btnAction }}
    <span>
      <box-icon name="chevron-right" color="white"></box-icon>
    </span>
  </button>
</template>

<script>
export default {
  name: "BtnPrimary",
  props: {
    btnAction: String,
  },
};
</script>

<style lang="scss">
.btn-primary {
  background-color: var(--c-orange);
  color: var(--c-white);
  display: flex;
  align-items: center;
  border: none;
  padding: 0.6em 0.5em 0.6em 0.9em;
  font-weight: var(--fweight-b);
  cursor: pointer;
  transition: 0.4s ease;
  span {
    margin-left: 0.5em;
  }
  &:hover {
    background-color: var(--c-orange-light);
    box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 15px -3px,
      rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;
    border-radius: 0.3em;
    transition: 0.4s ease;
  }
}
</style>
