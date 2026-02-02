<template>
  <div class="board-wrapper">
    <div class="chessboard">
      <div
        v-for="n in 64"
        :key="n"
        :class="['square', getColor(n)]"
      ></div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    getColor(n) {
      const row = Math.floor((n - 1) / 8)
      const col = (n - 1) % 8
      return (row + col) % 2 === 0 ? 'light' : 'dark'
    }
  }
}
</script>
