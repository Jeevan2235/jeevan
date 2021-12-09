<template>
  <div>
    <div v-for="link in links" :key="link">
      <h1 class="mt-8">Price Details-</h1>
      <p class="mt-3">
        <span style="font-weight: bold; font-size: 20px">Rent/Month:</span>
        {{ link.rent }}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px">Service Charge :</span>
        {{ link.charge }}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px"
          >Security Deposit :</span
        >
        {{ link.security }}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px"
          >Flat Release Policy :</span
        >
        {{ link.policy }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        rent: "$550 (negotiable)",
        charge: "8,000/= Tk per month, subject to change",
        security: "3 month’s rent",
        policy: "Policy",
      },
    ],
  }),
};
</script>

<style></style>
