<template>
  <div>
    <p>home</p>

    <button @click="getApi()">Chamar API</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    getApi() {
      fetch(`http://localhost:3333/teste`)
        .then((r) => r.json())
        .then((r) => console.log(r));
    },
  },
};
</script>
