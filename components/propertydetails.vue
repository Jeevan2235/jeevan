<template>
  <div>
    <div v-for="link in links" :key="link" style="padding-right:280px">
      <h1 class="mt-8">Property Details-</h1>
      <p class="mt-3">
        <span style="font-weight: bold; font-size: 20px">Address & Area :</span>
        {{link.Address}}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px">Flat Size :</span> {{link.Flat}}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px">Floor :</span> {{link.Floor}}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px">Room Category :</span>
        {{link.Category}}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px">Facilities :</span> 1
        {{link.Facilities}}
      </p>
      <p>
        <span style="font-weight: bold; font-size: 20px"
          >Additional Facilities
        </span>
      {{link.Additional}}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        Address: " Rangs Malancha, House-68, Road-6A (Dead End Road), Dhanmondi Residential Area.",
        Flat: "3000 Sq Feet.",
        Floor: "A5 (5th Floor) (6 storied Building ) (South Facing Unit)",
        Category: "3 Large Bed Rooms with 3 Verandas, Spacious Drawing, Dining & Family Living Room, Highly Decorated Kitchen with Store Room and Servant room with attached Toilet",
        Facilities: "1 Modern Lift, All Modern Amenities & Semi Furnished.",
        Additional: "Electricity with full generator load, b. Central Gas Geyser, c. 2 Car Parking with 1 Driver’s Accommodation, d. Community Conference Hall, e. Roof Top Beautified Garden and Grassy Ground, f. Cloth Hanging facility with CC camera",
      },
    ],
  }),
};
</script>

<style></style>
