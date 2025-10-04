# Introdução a Técnicas de Programação - Unidade 1

**Aluno**: Marcelo Augusto Gomes Bastos de Araújo
**Matrícula**: 20250033007
**Período**: 2025.2

## 📁 Estrutura do Projeto

- `projeto/`: Projeto principal da unidade
- `listas/`: Soluções das listas de exercícios
- `README.md`: Este arquivo

## 🚀 Projeto: Jogo da Velha com IA

**Descrição**: O projeto simula um jogo da velha de 3x3 onde um jogador humano ('X') compete contra o computador ('O'). O cerne do projeto reside na implementação do algoritmo Minimax, que garante que a IA sempre fará o melhor movimento possível, resultando em:

Vitória: Se houver um caminho garantido para vencer.

Empate: Se a vitória não for possível, garantindo no mínimo o empate.

**Repositório**: https://github.com/MarceloAraujo71/Entrega-U1-ITP.git

### Funcionalidades Implementadas:
- 1. Inicialização e Interface
inicializar_tabuleiro(): Prepara o tabuleiro 3x3, preenchendo todas as posições com espaços vazios (' ').

exibir_tabuleiro(): Apresenta o estado atual do tabuleiro de forma clara no console, usando caracteres de separação (|, -).

Entrada do Usuário: Gerencia a leitura das jogadas do jogador humano ('X'), validando se as coordenadas (Linha e Coluna) estão dentro dos limites (1 a 3) e se a posição escolhida está vazia.

2. Lógica do Jogo
tem_movimentos(): Verifica se ainda há espaços vazios disponíveis no tabuleiro. Usada para determinar a possibilidade de empate.

checar_vitoria(): Examina todas as linhas, colunas e diagonais do tabuleiro para determinar se algum jogador atingiu três em linha.

Retorna 10 se a IA ('O') venceu.

Retorna -10 se o Jogador ('X') venceu.

Retorna 0 se não há vencedor.

3. Inteligência Artificial (Algoritmo Minimax)
minimax(profundidade, maximizando_jogador): Esta é a função central que implementa o algoritmo Minimax de forma recursiva e com backtracking.

Simulação Completa: Avalia todas as possíveis jogadas futuras a partir do estado atual do jogo.

Maximização: Quando é a vez da IA, busca o movimento que maximize sua pontuação (INT_MIN).

Minimização: Quando é a vez do Jogador, assume que o humano fará o movimento que minimize a pontuação da IA (INT_MAX).

Otimização: Ajusta a pontuação final pela profundidade da jogada, incentivando vitórias mais rápidas e adiando derrotas.

encontrar_melhor_movimento(): Itera sobre todos os espaços vazios e usa a função minimax para calcular a pontuação de cada movimento possível. Seleciona e retorna o movimento que resulta no melhor valor Minimax para a IA.

### Conceitos da U1 Aplicados:
- Estruturas condicionais: checar_vitoria(); minimax(); main(); encontrar_melhor_movimento();
- Estruturas de repetição: inicializar_tabuleiro(); exibir_tabuleiro(); tem_movimentos(); checar_vitoria(); minimax(); encontrar_melhor_movimento();
- Vetores: char tabuleiro[3][3];
- Funções: inicializar_tabuleiro(); exibir_tabuleiro(); tem_movimentos(); checar_vitoria(); minimax(); encontrar_melhor_movimento();

## 📚 Listas de Exercícios

### Semana 2 - Variáveis, Tipos e Operadores:
- ✅ Problema 1: Calculadora de IMC
- ✅ Problema 2: Conversão de temperatura
- ✅ Problema 3: Cálculo de juros compostos
- ✅ Problema 4: Operações aritméticas básicas

### Semana 3 - Condicionais:
- ✅ Problema 1: Classificação de IMC
- ✅ Problema 2: Calculadora de energia elétrica
- ✅ Problema 3: Sistema de notas
- ✅ Problema 4: Pedra, papel, tesoura
- ✅ Problema 5: Calculadora de desconto progressivo
- ✅ Problema 6: Diagnóstico médico simples
- ✅ Problema 7: Sistema de equações do 2º grau
- ✅ Problema 8: Validador de triângulos

### Semana 4A - Repetições:
- ✅ Problema 1: Dobrar folha
- ✅ Problema 2: Homem Aranha
- ✅ Problema 3: Números colegas
- ✅ Problema 4: Jogo de dardos

### Semana 4B - Análise e Padrões:
- ✅ Questões 1-4: Análise de código
- ✅ Questões 5-11: Implementações

### Semana 5 - Funções (Parte 1):
- ✅ Problema 1: Horários das rondas
- ✅ Problema 2: Primos triplos
- ✅ Problema 3: Pousando a sonda espacial

### Semana 6 - Vetores:
- ✅ Problema 1: MEC - Correção ENEM
- ✅ Problema 2: Álbum de figurinhas
- ✅ Problema 3: A construção da ponte
- ✅ Problema 4: Em busca do tesouro perdido

## 🎯 Principais Aprendizados
[Reflita sobre os principais conceitos aprendidos na U1]

## 🔧 Ambiente de Desenvolvimento
- **SO**: Windows
- **Compilador**: GCC versão 8.1.0
- **Editor**: Visual Studio Code (VS Code)