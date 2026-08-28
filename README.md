# Calculadora de Saúde

## Descrição do Projeto

Este projeto é um sistema desenvolvido em Python para realizar cálculos simples relacionados à saúde e bem-estar.

O sistema possui as seguintes funcionalidades:

- Cálculo do IMC;
- Classificação do IMC;
- Recomendação diária de consumo de água;
- Cálculo da frequência cardíaca máxima;
- Menu interativo no terminal.

Durante os testes foram encontrados bugs no código original, que foram analisados e corrigidos.

## Relatório de Bugs Encontrados

| Local do Bug | Comportamento Incorreto Observado | Solução Aplicada |
|---|---|---|
| `calcular_imc()` | O cálculo utilizava `altura * 2` em vez de elevar a altura ao quadrado. | Alterado para `peso / (altura ** 2)`. |
| `classificar_imc()` | Alguns valores limites do IMC não recebiam classificação correta. | As condições foram ajustadas para considerar todas as faixas. |
| `calcular_agua_diaria()` | O peso era dividido por 35, gerando um valor incorreto. | Alterado para `(peso * 35) / 1000`, calculando o resultado em litros. |
| `calcular_frequencia_cardiaca_maxima()` | A idade era somada a 220. | Alterado para `220 - idade`. |
| `menu()` | O `input()` retornava texto e as opções eram comparadas com números. | A opção foi convertida para inteiro. |
| `main()` | As opções do menu não eram reconhecidas corretamente por causa do tipo de dado. | Ajustado o tratamento da variável `opcao`. |
| `main()` - opção 4 | O programa mostrava a mensagem de saída, mas continuava executando. | Adicionado `break` para encerrar o `while`. |

## Como Executar

Para executar o projeto, é necessário ter o Python instalado no computador.

Abra o terminal na pasta do projeto e execute:

```bash
python calculadora_saude.py
```

Depois será exibido o menu:

```text
1. Calcular IMC
2. Calcular Recomendação de Água
3. Calcular Frequência Cardíaca Máxima
4. Sair
```

Digite o número da opção desejada e siga as instruções exibidas no terminal.




