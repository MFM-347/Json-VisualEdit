<template>
  <div class="wf a">
    <div class="contain">
      <div class="window-controls">
        <div class="dot red"></div>
        <div class="dot yellow"></div>
        <div class="dot green"></div>
      </div>
      <div class="code-block">
        <p class="code-line keyword">const <span class="object">message</span> = {</p>
        <p class="code-line indent">type: <span class="string">'Error'</span>,</p>
        <p class="code-line indent">title: <span class="string">'404'</span>,</p>
        <p class="code-line indent">description: <span class="string">'Page Not Found'</span></p>
        <p class="code-line keyword">};</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.a {
  display: grid;
  place-items: center;
}
.contain {
  position: relative;
  margin: auto;
  width: clamp(400px, 90%, 500px);
  min-height: clamp(225px, 250px, 300px);
  height: 275px;
  max-height: 300px;
  padding: 1rem;
  border-radius: 1.5rem;
  background: #262626;
  border: 1px solid #404040;
  transition: all 0.3s ease-in-out;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.175);
  overflow: hidden;
}
.contain:hover {
  transform: scale(1.025);
  border-color: #385cfa;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.25);
}
.window-controls {
  position: absolute;
  display: flex;
  top: 12.5px;
  left: 12.5px;
  gap: 8px;
}
.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  transition: transform 0.2s;
}
.dot:hover {
  transform: scale(1.1);
}
.red {
  background: #fb2c36;
}
.yellow {
  background: #efb100;
}
.green {
  background: #00c951;
}
.code-block {
  margin-top: 1.5rem;
  font-size: clamp(12px, 1.2vw, 14px);
  font-family: 'Fira Code', monospace;
  line-height: 1.5;
  overflow: hidden;
  max-height: 12rem;
}
.keyword {
  color: #ae63e4;
}
.object {
  color: #ffdd40;
}
.string {
  color: #47cf73;
}
.indent {
  margin-left: 1.2rem;
}
</style>
