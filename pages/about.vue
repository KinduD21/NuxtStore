<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste eius nam
      nisi? Quae sint sed cum sapiente suscipit velit aliquam incidunt aut eos.
      Amet ex voluptas maxime non reiciendis libero.
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste eius nam
      nisi? Quae sint sed cum sapiente suscipit velit aliquam incidunt aut eos.
      Amet ex voluptas maxime non reiciendis libero.
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/currency/UAH");
</script>
