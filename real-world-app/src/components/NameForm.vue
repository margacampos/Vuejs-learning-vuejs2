<!-- eslint-disable prettier/prettier -->
<!-- eslint-disable vue/no-mutating-props -->
<template>
    <label for="name">
      Name your own route:
      <input type="text" id="name" :value="route" @input="$emit('change-route', $event.target.value)" />
    </label>
</template>
<!-- eslint-disable prettier/prettier -->

<script>
export default {
  props: ['route'],
  emits: ['change-route'],
  data: () => {
    return{
        name: "name"
    };
  },
  methods: {
    onSubmit(){
        this.$emit('change-route', this.name);
    }
  }
};
</script>
<!-- eslint-disable prettier/prettier -->

<style></style>
