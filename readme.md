# Calculadora LCOE Avançada

Este projeto é uma calculadora interativa para calcular o **LCOE (Levelized Cost of Energy)** de sistemas fotovoltaicos. A calculadora é construída com **HTML**, **CSS**, **JavaScript** e usa bibliotecas como **Bootstrap** e **Inputmask** para oferecer uma experiência de usuário otimizada e intuitiva.

## 📋 Índice
- [Visão Geral](#visão-geral)
- [Funcionalidades](#funcionalidades)
- [Pré-requisitos](#pré-requisitos)
- [Como Usar](#como-usar)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

## 🚀 Visão Geral

O LCOE é uma métrica usada para calcular o custo médio por unidade de energia gerada por um sistema ao longo de sua vida útil. Esta calculadora permite que você insira dados como investimento inicial, custos operacionais, taxa de desconto, geração de energia e vida útil para obter o resultado de forma fácil e precisa.

## ✨ Funcionalidades

- Máscaras de entrada para valores monetários, porcentagens e números.
- Suporte ao formato brasileiro para moedas e separadores decimais.
- Interface limpa e responsiva usando **Bootstrap 5**.
- Resultados exibidos em tempo real com cálculos precisos.
- Suporte para taxas de desconto e vida útil do projeto.

## ⚙️ Pré-requisitos

Certifique-se de ter um navegador moderno atualizado para executar este projeto.

## 🛠 Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/calculadora-lcoe.git
   cd calculadora-lcoe
   ```

2. Abra o arquivo index.html em qualquer navegador.

3. Preencha os campos do formulário:

- **Investimento Inicial (CAPEX):** O valor total do sistema em R$.
- Despesas Operacionais (OPEX): Custos anuais de operação do sistema em R$.
- Geração de Energia Anual (kWh): Energia gerada pelo sistema por ano em kWh.
- Taxa de Desconto (%): Percentual da taxa de desconto anual.
- Vida Útil do Projeto (anos): Quantos anos o projeto vai durar.

4. Clique em Calcular LCOE para visualizar o resultado.

## 💻 Tecnologias Utilizadas
- HTML5
- CSS3
- JavaScript (ES6+)
- Bootstrap 5 - Para o design responsivo.
- Inputmask - Para aplicar máscaras de entrada nos campos.

## 🧩 Exemplo de Uso

Após preencher os campos corretamente, o resultado do LCOE será exibido em formato monetário:
```
O LCOE é: R$ 0,50 por kWh
```
## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do repositório.
2. Crie uma branch para sua feature:

```
git checkout -b feature/sua-feature
```

3. Faça o commit das suas alterações:

```
git commit -m "Adiciona nova feature"
```

4. Envie para o seu fork:
```
git push origin feature/sua-feature
```

5. Abra um Pull Request.

## 📜 Licença

Este projeto está licenciado sob a MIT License. Sinta-se à vontade para usá-lo e modificá-lo!