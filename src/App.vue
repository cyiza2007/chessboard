<template>
  <div class="app-container">
    <!-- Sidebar -->
    <aside class="sidebar">
      <h2 class="logo">♟ GLORY <span>ACADEMY</span></h2>

      <ul class="menu">
        <li class="active">▶ Active Game</li>
        <li>Post-Match</li>
        <li>Puzzles</li>
        <li>Friends</li>
      </ul>

      <div class="resign">⛳ Resign</div>
    </aside>

    <!-- Main Content -->
    <main class="main">
      <header class="top-bar">
        <p>cyiza murenzi arnold</p>
        <small>Player 1 vs Player 2</small>
      </header>

      <!-- Chessboard -->
      <HelloWorld />

      <!-- Bottom info -->
      <div class="bottom-bar">
        <div class="player">
          <img src="https://i.pravatar.cc/40" />
          <span>Player 1</span>
        </div>

        <div class="timer">05:42</div>
      </div>
    </main>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: {
    HelloWorld
  }
}
</script>
