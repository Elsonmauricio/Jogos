Documentação do Projeto de Jogos Java
Visão Geral
Este projeto implementa um conjunto de jogos em Java com interface gráfica (Swing) e também uma versão de console para o jogo de Damas. O menu inicial permite ao usuário escolher entre:

Jogo de Damas (com interface gráfica e console)
Jogo das Bolas (interface gráfica)
Jogo de Perguntas e Respostas (interface gráfica)
Estrutura dos Arquivos
MenuInicial.java: Menu principal para seleção dos jogos.
DamasGUI.java: Interface gráfica do jogo de Damas.
JogoDamas.java: Versão console do jogo de Damas.
Tabuleiro.java: Lógica do tabuleiro e regras do jogo de Damas.
Peca.java: Representação de uma peça do jogo de Damas.
Main.java: Jogo das Bolas (interface gráfica).
JogoPerguntasRespostasGUI.java: Jogo de perguntas e respostas (interface gráfica).
Jogo de Damas
Classes Principais
1. Peca.java
Representa uma peça do jogo (branca ou preta, dama ou não).
Métodos:
isBranca(), isDama(), tornarDama(), toString(), etc.
2. Tabuleiro.java
Gerencia o estado do tabuleiro, peças, regras de movimento e captura.
Principais métodos:
getPeca(linha, coluna): Retorna a peça em uma posição.
validarMovimento(...): Valida se um movimento é permitido.
moverPeca(...): Move uma peça e trata capturas/promoções.
existeCapturaDisponivel(...), getPecasComCapturaObrigatoria(): Regras de captura obrigatória.
verificarVitoria(): Detecta fim de jogo.
imprimirTabuleiro(): Mostra o tabuleiro no console.
3. DamasGUI.java
Interface gráfica do jogo de Damas.
Exibe o tabuleiro, permite seleção/movimento de peças, destaca movimentos válidos e capturas obrigatórias.
Permite retornar ao menu inicial.
4. JogoDamas.java
Versão console do jogo de Damas.
Permite jogar via terminal, digitando coordenadas.
Jogo das Bolas
Main.java
Interface gráfica onde o usuário pode clicar em bolas coloridas para "explodi-las".
Quando 6 bolas de uma cor são removidas, o jogo reinicia.
Permite retornar ao menu inicial.
Jogo de Perguntas e Respostas
JogoPerguntasRespostasGUI.java
Interface gráfica para perguntas de múltipla escolha.
Mostra perguntas, opções, pontuação e resultado final.
Permite retornar ao menu inicial.
Menu Inicial
MenuInicial.java
Tela inicial com botões para acessar cada jogo.
Fecha o menu ao abrir um jogo e permite retornar ao menu a partir dos jogos.
Como Executar
Compile todos os arquivos Java:
Execute o menu inicial:
Para rodar o jogo de Damas no console:
Observações
O projeto utiliza apenas bibliotecas padrão do Java (Swing, AWT).
Não há uso de pacotes (package), então todos os arquivos devem estar na mesma pasta.
O código está preparado para rodar tanto em modo gráfico quanto console (para Damas).
Autor:
   Elson Mauricio
Data: 12/04/2025
