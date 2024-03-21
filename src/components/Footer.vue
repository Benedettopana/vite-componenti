<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },

  methods: {
    contatore() {
      setInterval(() => {
        this.counter++;
      }, 1000);
    },
  },

  mounted() {
    console.log("footer montato");
    this.contatore();
  },
};
</script>

<template>
  <div>contatore: {{ counter }}</div>
</template>

<style scoped></style>
