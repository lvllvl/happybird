<template>
  <div class="menu">
    <h1>happy bird</h1>
    <button @click="startGame">start game</button>
    <button @click="viewHighScores">high scores</button>
    <button @click="viewSettings">settings</button>
  </div>
</template>

<script>
export default {
  methods: {
    startGame() {
      // Logic to start the game
      this.$router.push('/game');
    },
    viewHighScores() {
      // Logic to view high scores
      this.$router.push('/highScores');
    },
    viewSettings() {
      // Logic to view settings
        this.$router.push('/settings');
    }
  }
}
</script>

<style scoped>
.menu {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

h1 {
  font-size: 48px;
  margin-bottom: 20px;
}

button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}

button:hover {
  background-color: white;
  color: black;
  border: 2px solid #4CAF50;
}
</style>
