<template>
    <div>
      <h2>Danh sách ngày trong tuần:</h2>
      <ul>
        <li v-for="(day, index) in days" :key="index">
          {{ index + 1 }}. {{ day }}
        </li>
      </ul>
    </div>


    <div>
        <h2>Danh sách số:</h2>
        <ul style="display: flex;gap: 10px;list-style: none;">
          <li v-for="(number, index) in numbers" :key="index">
            {{ number }}
          </li>
        </ul>
        <button @click="addNumber">Thêm số ngẫu nhiên</button>
      </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        days: ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
        numbers: [1, 2, 3, 4, 5],
      };
    },
    methods: {
    addNumber() {
      this.numbers.push(Math.floor(Math.random() * 100) + 1);
    },
  },
  };
  </script>

  
  