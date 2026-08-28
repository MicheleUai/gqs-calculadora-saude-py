# 🩺 Calculadora de Saúde

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Corrigido-success)
![Projeto](https://img.shields.io/badge/Projeto-Acad%C3%AAmico-purple)
![Git](https://img.shields.io/badge/Git-Versionamento-orange)

---

## 📌 Descrição do Projeto

Este projeto é um sistema desenvolvido em **Python** para realizar cálculos simples relacionados à saúde e bem-estar.

O objetivo da atividade foi analisar o código original, identificar falhas, corrigir os bugs encontrados e documentar todas as alterações realizadas.

### ✨ Funcionalidades

- ⚖️ Cálculo do IMC;
- 📊 Classificação do IMC;
- 💧 Recomendação diária de consumo de água;
- ❤️ Cálculo da frequência cardíaca máxima;
- 💻 Menu interativo executado pelo terminal.

---

## 🐞 Relatório de Bugs Encontrados

| Nº | Local do Bug | Comportamento Incorreto Observado | Solução Aplicada |
|---:|---|---|---|
| 1 | `calcular_imc()` | O cálculo utilizava `altura * 2` em vez de elevar a altura ao quadrado. | Alterado para `peso / (altura ** 2)`. |
| 2 | `classificar_imc()` | Alguns valores limites do IMC poderiam ficar sem classificação. | As condições foram ajustadas para cobrir corretamente todas as faixas. |
| 3 | `calcular_agua_diaria()` | O peso era dividido por 35, gerando resultado incorreto. | Alterado para `(peso * 35) / 1000`, retornando o valor em litros. |
| 4 | `calcular_frequencia_cardiaca_maxima()` | A idade era somada a 220. | Alterado para `220 - idade`. |
| 5 | `menu()` | O `input()` retornava texto, mas as opções eram comparadas com números inteiros. | A opção do menu passou a ser convertida para inteiro. |
| 6 | `main()` | As opções do menu não eram reconhecidas corretamente devido ao tipo de dado. | Ajustado o tratamento da variável `opcao`. |
| 7 | `main()` - opção 4 | O programa mostrava a mensagem de encerramento, mas permanecia no loop. | Adicionado `break` para encerrar o programa corretamente. |

---

## ✅ Correções Realizadas

Após as correções:

- ✅ O cálculo do IMC passou a utilizar a fórmula correta;
- ✅ As faixas de classificação do IMC foram ajustadas;
- ✅ A recomendação diária de água passou a retornar o resultado em litros;
- ✅ O cálculo da frequência cardíaca máxima foi corrigido;
- ✅ O menu passou a reconhecer corretamente as opções digitadas;
- ✅ A opção de saída encerra o programa normalmente;
- ✅ Todas as funcionalidades do menu podem ser executadas sem interromper o sistema.

---

## ▶️ Como Executar

### Pré-requisitos

É necessário ter o **Python 3** instalado no computador.

### 1. Clone o repositório

```bash
git clone https://github.com/MicheleUai/gqs-calculadora-saude-py.git
```

### 2. Entre na pasta do projeto

```bash
cd gqs-calculadora-saude-py
```

### 3. Execute o programa

```bash
python calculadora_saude.py
```

---

## 🖥️ Menu do Sistema

Ao executar o programa, será exibido:

```text
==============================
  SISTEMA DE SAÚDE E BEM-ESTAR
==============================
1. Calcular IMC
2. Calcular Recomendação de Água
3. Calcular Frequência Cardíaca Máxima
4. Sair
```

Digite o número da opção desejada e siga as instruções exibidas no terminal.

---

## 🛠️ Tecnologias Utilizadas

- 🐍 Python
- 🌿 Git
- 🐙 GitHub
- 📝 Markdown
- 💻 Visual Studio Code

---

## 📚 Objetivo Acadêmico

Atividade desenvolvida com foco em:

- identificação de bugs;
- correção de erros de lógica;
- análise de fluxo de execução;
- documentação técnica;
- boas práticas de versionamento com Git e GitHub.

---

## 👩‍💻 Autores

- Michele Carvalho
- Isaque Guimaraes

Projeto desenvolvido para atividade acadêmica de análise e correção de bugs em Python.







