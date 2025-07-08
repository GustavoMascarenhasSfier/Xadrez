
# ♟️ Jogo de Xadrez em C

Este é um projeto completo de **jogo de xadrez** desenvolvido em **linguagem C**, com foco em lógica, estrutura de dados, interação via terminal e persistência de dados. O jogo inclui:

- Sistema de **login e cadastro de usuários**
- **Ranking de jogadores** com pontuação baseada em vitórias e empates
- **Salvamento e retomada** de partidas
- **IA adversária** com jogadas automáticas (modo contra o computador)
- Interface de **terminal** com suporte a cores via ANSI

---

## 🧠 Funcionalidades

- ♟️ Jogo de xadrez completo com regras básicas e promoção de peão
- 👤 Cadastro e login de usuários (com armazenamento em `usuarios.txt`)
- 🏆 Ranking ordenado por pontuação (3 pontos por vitória, 1 por empate)
- 💾 Salvar e retomar partidas (`partida_salva.txt`)
- 🤖 Jogador preto sempre controlado por **IA adversária**
- ✅ Detecção de **xeque** e **xeque-mate**
- 🎨 Exibição colorida das peças no terminal

---

## 🚀 Como Executar

### 📋 Requisitos

- Compilador C (`gcc`) instalado no sistema

### 💻 Compilar

```bash
gcc xadrez.c -o xadrez
```

### ▶️ Executar

```bash
./xadrez       # Linux/macOS
xadrez.exe     # Windows (caso compilado com MinGW)
```

---

## 📁 Estrutura de Arquivos

```
xadrez.c               # Código-fonte principal
usuarios.txt           # Arquivo com login/senha e estatísticas dos jogadores
partida_salva.txt      # Estado salvo da partida em andamento
```

---

## 📋 Menu Principal

```
=== MENU PRINCIPAL ===
1. Jogar nova partida
2. Retomar partida salva
3. Ver ranking
4. Cadastrar novo usuário
5. Sair
```

---

## 💾 Dados Salvos

- `usuarios.txt`: formato:
  ```
  nome senha vitorias derrotas empates
  ```
- `partida_salva.txt`: contém o tabuleiro atual e o jogador da vez

---

## 🧮 Regras do Ranking

- Vitória: +3 pontos
- Empate: +1 ponto
- Derrota: 0 pontos

Ranking ordenado por pontuação total.

---

## 🛠️ Tecnologias e Conceitos

- Linguagem **C**
- **Structs** para representar peças, casas e usuários
- **Manipulação de arquivos** (`fopen`, `fprintf`, `fscanf`)
- **IA adversária simples** com heurística de pontuação
- **Controle de jogadas e regras do xadrez**
- **ANSI codes** para colorir o terminal

---

## 🧪 Melhorias Futuras

- Adição de **movimentos especiais** (roque, en passant)
- Detecção de empate por repetição ou falta de material
- Interface gráfica (por exemplo, com `ncurses`)
- Exportação de histórico de partidas

---

## 👨‍💻 Autor

Desenvolvido por **Gustavo Mascarenhas**  
Projeto acadêmico com fins educativos e de prática em lógica de programação, C e algoritmos.
