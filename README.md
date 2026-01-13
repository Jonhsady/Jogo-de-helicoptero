# 🚁 Jogo de Helicóptero - Resgate

Um jogo de ação desenvolvido com JavaScript e jQuery onde você pilota um helicóptero Apache em missões de resgate. Resgate seus aliados, elimine inimigos e sobreviva o máximo possível!

## 🎮 Sobre o Jogo

Você é o piloto de um helicóptero Apache em uma missão de resgate perigosa. Seu objetivo é:
- ✅ **Resgatar** o máximo de aliados possível
- 🎯 **Eliminar** inimigos com seus disparos
- ⚡ **Sobreviver** mantendo sua energia acima de zero
- 📈 **Acumular** pontos para bater seu recorde

## 🎯 Funcionalidades

- **Sistema de Pontuação:**
  - Pontos por eliminar inimigos (50-100 pontos)
  - Contador de aliados salvos
  - Contador de aliados perdidos
  - Pontuação em tempo real

- **Sistema de Energia:**
  - 3 níveis de energia inicial
  - Perde energia ao colidir com inimigos
  - Game Over quando energia chega a zero

- **Elementos do Jogo:**
  - 🚁 Helicóptero Apache (jogador)
  - 👤 Aliado para resgatar
  - 🎯 Inimigo tipo 1 (movimento vertical aleatório)
  - 🎯 Inimigo tipo 2 (movimento horizontal)
  - 💥 Animações de explosão
  - 🎵 Música de fundo e efeitos sonoros

- **Efeitos Visuais:**
  - Animações de sprites
  - Fundo em movimento
  - Efeitos de explosão
  - Interface visual atrativa

## 🕹️ Como Jogar

### Controles:
- **W** - Move o helicóptero para **CIMA**
- **S** - Move o helicóptero para **BAIXO**
- **D** - **DISPARA** mísseis

### Objetivos:
1. **Resgatar Aliados:** Colida com o aliado para resgatá-lo
2. **Eliminar Inimigos:** Use os disparos (tecla D) para destruir os inimigos
3. **Evitar Colisões:** Não colida com os inimigos ou perderá energia
4. **Proteger Aliados:** Evite que os inimigos atinjam os aliados

### Dicas:
- Eliminar inimigos aumenta a velocidade do jogo (dificuldade progressiva)
- Inimigo tipo 1 vale mais pontos (100) que o tipo 2 (50)
- Mantenha-se sempre em movimento para evitar colisões
- Use os disparos estrategicamente

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura do jogo
- **CSS3** - Estilização e animações
- **JavaScript** - Lógica do jogo
- **jQuery** - Manipulação do DOM
- **jQuery Collision** - Detecção de colisões

## 📦 Como Executar

### Opção 1: Abrir diretamente
```bash
# Simplesmente abra o arquivo index.html no seu navegador
```

### Opção 2: Servidor local (recomendado)
```bash
# Com Python 3
cd Jogo-de-helicoptero
python3 -m http.server 8000

# Acesse: http://localhost:8000
```

### Opção 3: Com Node.js
```bash
# Instale o http-server globalmente (se necessário)
npm install -g http-server

# Execute
cd Jogo-de-helicoptero
http-server

# Acesse: http://localhost:8080
```

## 📁 Estrutura do Projeto

```
Jogo-de-helicoptero/
├── index.html          # Página principal do jogo
├── css/
│   └── estilos.css     # Estilos e animações
├── js/
│   ├── js.js           # Lógica principal do jogo
│   ├── jquery-1.11.1.min.js      # Biblioteca jQuery
│   └── jquery-collision.min.js   # Plugin de colisão
├── imgs/               # Imagens e sprites do jogo
│   ├── apache.png      # Helicóptero do jogador
│   ├── helicoptero.png # Sprite animado do helicóptero
│   ├── inimigo1.png    # Inimigo tipo 1
│   ├── inimigo2.png    # Inimigo tipo 2
│   ├── amigo.png       # Aliado para resgatar
│   ├── amigo_morte.png # Animação de morte do aliado
│   ├── explosao.png    # Sprite de explosão
│   ├── disparo.png     # Projétil
│   ├── energia0-3.png  # Indicadores de energia
│   ├── fundo.jpg       # Fundo da página
│   └── fundo_game.jpg  # Fundo do jogo
├── sons/               # Efeitos sonoros e música
│   ├── som.mp3         # Som de disparo
│   ├── explosao.mp3    # Som de explosão
│   ├── musica_fundo.mp3 # Música de fundo
│   ├── gameover.mp3    # Som de game over
│   ├── perdido.mp3     # Som quando aliado é perdido
│   └── resgate.mp3     # Som de resgate bem-sucedido
├── fontes/             # Fontes personalizadas
│   └── ANODETONOONE.TTF
└── README.md           # Este arquivo
```

## 🎯 Mecânicas do Jogo

### Sistema de Pontuação:
- **Eliminar Inimigo 1:** +100 pontos
- **Eliminar Inimigo 2:** +50 pontos
- **Resgatar Aliado:** +1 no contador de salvos
- **Aliado Perdido:** +1 no contador de perdidos

### Sistema de Energia:
- **Energia Inicial:** 3
- **Perda de Energia:** -1 ao colidir com qualquer inimigo
- **Game Over:** Quando energia chega a 0

### Dificuldade:
- A velocidade aumenta gradualmente ao eliminar inimigos
- Inimigos aparecem em posições aleatórias
- Aliados e inimigos reaparecem após serem coletados/eliminados

## 🎨 Características Técnicas

- **Animações:** CSS3 keyframes para sprites animados
- **Colisões:** jQuery Collision plugin para detecção precisa
- **Sons:** HTML5 Audio API para efeitos sonoros e música
- **Game Loop:** setInterval para atualização contínua (30ms)
- **Responsivo:** Layout fixo otimizado para 950x630px

## 🌟 Diferenciais

- ✅ Sistema completo de pontuação e estatísticas
- ✅ Múltiplos tipos de inimigos com comportamentos diferentes
- ✅ Sistema de energia/vida
- ✅ Efeitos sonoros e música de fundo
- ✅ Animações fluidas de sprites
- ✅ Sistema de resgate de aliados
- ✅ Dificuldade progressiva

## 📝 Notas

- O jogo funciona completamente offline (sem dependências externas)
- Todos os recursos (imagens, sons, fontes) estão incluídos no projeto
- Compatível com navegadores modernos que suportam HTML5 Audio

## 🎮 Screenshots

O jogo apresenta:
- Tela inicial com instruções
- Gameplay com helicóptero, inimigos e aliados
- Sistema de placar em tempo real
- Indicador de energia visual
- Tela de Game Over com opção de reiniciar

## 📄 Licença

Este projeto é de código aberto e está disponível para uso pessoal e educacional.

---

**Boa sorte na missão de resgate! 🚁🎮**

