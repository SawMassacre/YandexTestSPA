<template>
  <div>
    <input type="number" v-model="doorsCount" min="3" />
    <div class="doors">
      <svg
        v-for="(door, idx) in doors"
        :key="idx"
        @click="selectDoor(idx)"
        :class="{ open: door.open, selected: door.selected }"
      >
        <!-- Here goes your SVG for door -->
        <text v-if="door.car" :x="x" :y="y">Car</text>
        <text v-else :x="x" :y="y">Goat</text>
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      doorsCount: 3,
      doors: [],
    };
  },
  watch: {
    doorsCount(newVal) {
      if (newVal > 2) this.initializeDoors(newVal);
    },
  },
  methods: {
    initializeDoors(count) {
      let doors = [];
      let carIdx = Math.floor(Math.random() * count);
      for (let i = 0; i < count; i++) {
        doors.push({
          car: i === carIdx,
          open: false,
          selected: false,
        });
      }
      this.doors = doors;
    },
    selectDoor(idx) {
      for (let i = 0; i < this.doors.length; i++) {
        if (i !== idx && !this.doors[i].car) this.doors[i].open = true;
      }
      this.doors[idx].selected = true;
    },
  },
  created() {
    this.initializeDoors(this.doorsCount);
  },
};
</script>
