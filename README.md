# Cartas-Super-Trunfo
Desafio que visa criar um conjunto de " cartas " no formato Super Trunfo, onde o tema será Linguagens de Programação.

# 🃏 Desafio Super Trunfo: Linguagens de Programação

Este projeto é um desafio de estruturação de dados no formato do famoso jogo de cartas Super Trunfo, utilizando as Linguagens de Programação como tema central.

O objetivo é criar um *dataset* padronizado que possa ser consumido por qualquer aplicação futura (web, CLI, etc.) que queira simular o jogo.

## 🎯 Objetivo do Jogo

O jogo Super Trunfo consiste em comparar características entre duas cartas. O jogador que tiver o **maior** valor na categoria escolhida vence a rodada, exceto para atributos onde o **menor** valor é considerado superior (Regra Inversa).

**Neste desafio, a regra geral é: MAIOR VALOR VENCE, EXCETO ONDE ESPECIFICADO.**

## ⚙️ Os Atributos (e Regras de Vitória)

Todas as categorias utilizam uma escala de **1 a 100**, onde 100 representa o valor máximo/melhor.

| Característica | Regra de Vitória | Descrição e Critério |
| :--- | :--- | :--- |
| **Curva de Aprendizado** | **MENOR** valor vence (Regra Inversa) | Quão complexa é a sintaxe e o ecossistema para um iniciante. **Valor mais baixo = Mais Fácil.** |
| **Popularidade** | **MAIOR** valor vence | Baseado na relevância e uso no mercado (ex: índices TIOBE, Stack Overflow Survey). |
| **Performance (Velocidade)** | **MAIOR** valor vence | Velocidade de execução e capacidade de processamento (tempo de resposta). |
| **Comunidade (Suporte)** | **MAIOR** valor vence | Tamanho da comunidade, facilidade em encontrar tutoriais, documentação e suporte. |
| **Usabilidade em Back-end** | **MAIOR** valor vence | Quão popular, eficiente e escalável a linguagem é para o desenvolvimento de servidores e APIs. |

## 📦 Estrutura do Projeto

O deck de cartas está contido no arquivo JSON, que segue o seguinte formato:

- **Arquivo:** `cartas.json`
- **Estrutura de cada carta:**
```json
{
  "id": "Um código único da carta (ex: A1, B2)",
  "nome": "Nome da Linguagem",
  "descricao": "Breve resumo da linguagem",
  "atributos": {
    "curva_aprendizado": 0, // 1 a 100
    "popularidade": 0,      // 1 a 100
    "performance": 0,       // 1 a 100
    "comunidade": 0,        // 1 a 100
    "backend": 0            // 1 a 100
  }
}


