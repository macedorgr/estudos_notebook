# 🧠 Segundo Cérebro: Modelagem Financeira 2.0 e o Padrão FAST

## 🎯 Tema e Objetivo
> **"Construir uma base de conhecimento interativa sobre Modelagem Financeira 2.0, aplicando o padrão FAST e ferramentas modernas de IA para transformar planilhas determinísticas em sistemas de inteligência corporativa integrados."**

O objetivo deste projeto é estruturar um especialista virtual capaz de responder dúvidas complexas sobre finanças corporativas, análise de demonstrativos (3SM), transição IFRS 18, simulações estocásticas de Monte Carlo e uso de IA/Python no ecossistema de FP&A, utilizando exclusivamente fontes confiáveis e auditáveis.

---

## 📚 Fontes Utilizadas e Rationale de Confiança

1. **`Modelagem_Financeira_2.0.pdf` (Apresentação Principal)**
   * **Por que confio:** Documento estruturado que sintetiza os pilares de FP&A moderno, a nova arquitetura do IFRS 18, a metodologia de modelagem FAST, diagnósticos de liquidez/solidez e integração com Python e Claude IA. É o guia conceitual e prático de referência do projeto.
2. **`NotebookLM Mind Map.jpg` (Mapa Mental do Ecossistema)**
   * **Por que confio:** Mapeamento visual hierárquico das conexões entre fundamentos de contabilidade (3SM, Corkscrew), diretrizes FAST, análise de sensibilidade estocástica e stack tecnológica do Analista 2.0.
3. **`flashcards.csv` (Base de Conceitos e Flashcards)**
   * **Por que confio:** Base de dados objetiva contendo perguntas e respostas diretas sobre termos técnicos, métricas (EBITDA, NWC, PMR/PMP) e boas práticas de modelagem sem ambiguidade.
4. **`Áudio de Visão Geral (Resumo em Áudio)`**
   * **Por que confio:** Síntese executiva focada na relevância da transparência, auditabilidade e eliminação de erros na modelagem corporativa para alta gestão.

---

## 🤖 Diretriz de Comportamento (System Prompt do Notebook)

A seguinte diretriz foi fornecida ao NotebookLM para governar suas respostas:

```text
Você é um Especialista Sênior em Modelagem Financeira e FP&A 2.0. 
Sua função é responder a dúvidas técnicas sobre contabilidade corporativa, o padrão FAST de modelagem, transição IFRS 18, análise estocástica e integração de IA/Python no ambiente financeiro.

Regras estritas de comportamento:
1. Responda SEMPRE com base exclusivamente nas fontes fornecidas.
2. Não invente premissas nem utilize conhecimentos externos não contidos nos documentos.
3. Em todas as respostas, cite explicitamente de qual fonte (página do PDF, mapa mental ou flashcards) a informação foi extraída.
4. Mantenha um tom profissional, analítico e instrucional.
```

---

## ❓ Perguntas, Respostas e Evidências de Fontes

### Pergunta 1: O que é o Padrão FAST e quais são os seus 4 pilares na modelagem financeira?
* **Resposta do NotebookLM:**
  > O padrão **FAST** é uma metodologia institucional de arquitetura de modelagem financeira que exige transparência e estrutura de software nas planilhas. Os 4 pilares são:
  > * **F (Flexible / Flexível):** Abas organizadas logicamente por *Inputs*, *Cálculos* e *Outputs*.
  > * **A (Appropriate / Apropriado):** Foco nos macro-direcionadores de valor, evitando falsas precisões e complexidades desnecessárias.
  > * **S (Structured / Estruturado):** Fluxo temporal consistente (da esquerda para a direita) e ausência de lógica circular.
  > * **T (Transparent / Transparente):** Fórmulas curtas, cálculos isolados com links diretos, proibição de linhas/colunas ocultas e de referências circulares.
* **Fonte(s) Citada(s):** `Modelagem_Financeira_2.0.pdf` (Página 6) e `NotebookLM Mind Map.jpg` (Ramo: Fundamentos FAST).

---

### Pergunta 2: Quais são as principais mudanças introduzidas pelo IFRS 18 na DRE em comparação com o CPC 26?
* **Resposta do NotebookLM:**
  > O novo padrão **IFRS 18** (com vigência prevista para 2027) substitui a estrutura tradicional do CPC 26 ao categorizar o resultado em 5 seções bem definidas:
  > 1. **Operacional:** Essência do negócio (Receitas, Custos e Despesas Operacionais, gerando o Lucro Operacional).
  > 2. **Investimento:** Rendimentos e resultados de investimentos de longo prazo.
  > 3. **Financiamento:** Despesas e receitas atreladas à estrutura de capital.
  > 4. **Tributos:** Impostos diretos (IRPJ e CSLL).
  > 5. **Operações Descontinuadas:** Resultados de operações encerradas.
  > 
  > Essa alteração elimina subtotais livres e variáveis, criando uma métrica padronizada de Lucro Operacional.
* **Fonte(s) Citada(s):** `Modelagem_Financeira_2.0.pdf` (Página 3).

---

### Pergunta 3: Qual é o prompt padrão sugerido para utilizar o Claude IA como Co-piloto Financeiro em análises de variação?
* **Resposta do NotebookLM:**
  > Para realizar uma análise de variação (Realizado vs. Orçado vs. Ano Anterior) via Claude IA, deve-se utilizar a seguinte estrutura de prompt:
  > * **Contexto:** *"Aja como meu Especialista Financeiro..."*
  > * **Comando:** *"Faça análise Realizado x Orçado x Ano Anterior."*
  > * **Diretriz:** *"Isole Preço x Volume x Mix; Explique a variação de Margem Bruta."*
  > * **Classificação:** *"Separe em Favorável / Desfavorável / Neutro."*
  > * **Saída:** *"Gere Resumo Executivo + Tabela com Recomendações de Ação."*
* **Fonte(s) Citada(s):** `Modelagem_Financeira_2.0.pdf` (Página 9).

---

### Pergunta 4: Qual a diferença entre Análise de Sensibilidade e Simulação de Monte Carlo na modelagem estocástica?
* **Resposta do NotebookLM:**
  > * **Análise de Sensibilidade (Diagrama de Tornado):** Isola o impacto marginal de variáveis individuais (ex: variação de $+30\%$ a $-70\%$ na Margem Bruta ou de $+12\%$ a $-20\%$ no Preço de Venda), identificando os fatores que respondem pela maior parte da variância do resultado (regra 80/20).
  > * **Simulação de Monte Carlo:** Substitui premissas determinísticas por milhares de distribuições probabilísticas combinadas, revelando a probabilidade real de atingir determinado saldo de caixa projetado (métricas P50, P80, P90).
* **Fonte(s) Citada(s):** `Modelagem_Financeira_2.0.pdf` (Página 7) e `flashcards.csv`.

---

## 🔗 Link do Notebook Compartilhado

* **Link de acesso ao NotebookLM:** [Acessar Notebook no Google NotebookLM](https://notebook.google.com/notebook/26c0880b-649b-438b-9703-ff2842e43a96)

---

## 📁 Arquivos do Repositório

* `README.md` - Documentação central do Segundo Cérebro.
* `Modelagem_Financeira_2.0.pdf` - Apresentação técnica sobre o tema.
* `NotebookLM Mind Map.jpg` - Mapa mental do ecossistema de modelagem e FAST.
* `flashcards.csv` - Base de conhecimento em pares de pergunta/resposta.
* `prints/` - Pasta com screenshots comprobatórios das citações e respostas no chat do NotebookLM.