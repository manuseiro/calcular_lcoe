# Calculadora LCOE

Este é um projeto de uma calculadora LCOE (Levelized Cost of Energy) implementada em HTML e JavaScript. O LCOE é uma métrica comumente utilizada na indústria de energia para avaliar o custo médio de geração de energia ao longo do tempo.

## Cálculo do LCOE

A calculadora LCOE utiliza os valores fornecidos pelo usuário para calcular o LCOE (Levelized Cost of Energy), que é o custo médio de geração de energia ao longo do tempo. O cálculo é realizado da seguinte maneira:

1. São obtidos os seguintes valores do formulário preenchido pelo usuário:
   - **Investimento do Sistema:** Valor do investimento realizado no sistema de geração de energia.
   - **Despesas de Operação:** Valor das despesas operacionais do sistema.
   - **Despesas de Manutenção:** Valor das despesas de manutenção do sistema.
   - **Total de Eletricidade Gerada:** Valor total de eletricidade gerada pelo sistema.

2. O LCOE é calculado usando a fórmula:
```
LCOE = (Investimento + Despesas de Operação + Despesas de Manutenção) / Total de Eletricidade Gerada
```
3. O resultado é exibido na página, mostrando o custo médio de geração de energia (LCOE).

É importante ressaltar que os valores inseridos nos campos do formulário são convertidos em números decimais para garantir a precisão do cálculo do LCOE.

## Código JavaScript da Calculadora LCOE

```javascript
$(document).ready(function() {
  $('#lcoeForm').on('submit', function(event) {
    event.preventDefault(); // Impede o envio do formulário

    // Obtém os valores dos campos
    var investment = parseFloat($('#investmentInput').val());
    var operatingExpenses = parseFloat($('#operatingExpensesInput').val());
    var maintenanceExpenses = parseFloat($('#maintenanceExpensesInput').val());
    var totalElectricity = parseFloat($('#totalElectricityInput').val());

    // Calcula o LCOE
    var lcoe = (investment + operatingExpenses + maintenanceExpenses) / totalElectricity;

    // Exibe o resultado
    $('#result').html('<h3>O LCOE é: ' + lcoe.toFixed(2) + '</h3>');
  });
});
```

## Como usar

1. Abra o arquivo `index.html` em um navegador web compatível.
2. Preencha os seguintes campos do formulário:

   - **Investimento do Sistema:** Insira o valor do investimento realizado no sistema de geração de energia.
   - **Despesas de Operação:** Insira o valor das despesas operacionais do sistema.
   - **Despesas de Manutenção:** Insira o valor das despesas de manutenção do sistema.
   - **Total de Eletricidade Gerada:** Insira o valor total de eletricidade gerada pelo sistema.

3. Clique no botão "Calcular".

O resultado do cálculo do LCOE será exibido abaixo do botão "Calcular", indicando o custo médio de geração de energia.

## Tecnologias utilizadas

- HTML
- CSS (Bootstrap 5.3.0)
- JavaScript (jQuery 3.6.0)

## Observações

- Certifique-se de ter uma conexão com a internet para carregar as bibliotecas do Bootstrap e jQuery.
- O cálculo do LCOE é feito automaticamente quando o formulário é enviado. Os valores inseridos nos campos são convertidos em números decimais para garantir a precisão do cálculo.
