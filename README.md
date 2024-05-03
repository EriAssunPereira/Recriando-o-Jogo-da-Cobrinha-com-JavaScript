# Recriando-o-Jogo-da-Cobrinha-com-JavaScript

Claro, vou te guiar na criação do clássico Jogo da Cobrinha utilizando **HTML**, **CSS** e **JavaScript**. Vamos estruturar o projeto em módulos para manter o código organizado e fácil de manter.

### Descrição do Projeto:
O objetivo é desenvolver o Jogo da Cobrinha, onde o jogador controla uma cobra que cresce ao comer itens que aparecem na tela. O jogo termina se a cobra colidir com ela mesma ou com as bordas da área de jogo.

### Módulos:
1. **Motor do Jogo (Game Engine):**
   - Responsável pela lógica principal do jogo, como iniciar, pausar e terminar o jogo.
   - Controla o loop do jogo usando `requestAnimationFrame` para atualizações suaves.

2. **Renderização (Rendering):**
   - Usa o elemento `canvas` do HTML5 para desenhar a cobra e a comida na tela.
   - Atualiza a tela a cada frame do jogo.

3. **Controle da Cobra (Snake Control):**
   - Gerencia o movimento da cobra, incluindo mudanças de direção e crescimento ao comer.

4. **Gestão de Eventos (Event Management):**
   - Lida com eventos do teclado para controlar a direção da cobra.
   - Pode ser expandido para incluir eventos de toque em dispositivos móveis.

5. **Lógica da Comida (Food Logic):**
   - Posiciona aleatoriamente a comida na tela.
   - Verifica se a cobra comeu a comida para incrementar o tamanho.

6. **Pontuação e Níveis (Scoring and Levels):**
   - Mantém a pontuação do jogador e aumenta a dificuldade à medida que o jogo progride.

### Exemplo Prático:
Aqui está um exemplo básico de como você pode começar a estruturar seu código em módulos:

```javascript
// motor.js
export function iniciarJogo() {
  // Inicia o jogo
}

export function pausarJogo() {
  // Pausa o jogo
}

// renderizacao.js
export function desenharCobra(contexto, cobra) {
  // Desenha a cobra no canvas
}

export function desenharComida(contexto, comida) {
  // Desenha a comida no canvas
}

// controleCobra.js
export function moverCobra(cobra) {
  // Atualiza a posição da cobra
}

// gestaoEventos.js
export function configurarControles() {
  // Configura os controles do teclado
}

// comida.js
export function posicionarComida() {
  // Posiciona a comida de forma aleatória
}

// pontuacao.js
export function atualizarPontuacao(pontos) {
  // Atualiza a pontuação do jogador
}
```

Para integrar esses módulos, você usará `import` e `export` para compartilhar funcionalidades entre eles. Lembre-se de que cada módulo deve ter uma responsabilidade única, o que facilita a manutenção e a compreensão do código.

https://github.com/SpruceGabriela/snake-the-game
