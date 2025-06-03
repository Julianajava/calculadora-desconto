# calculadora-desconto
Projeto simples de uma calculadora de desconto feita em HTML, CSS e JavaScript.
# Calculadora de Desconto 🧮

Projeto simples feito com HTML, CSS e JavaScript que calcula o valor final de um produto após aplicar um desconto.

## 🚀 Funcionalidades
- Entrada do valor original
- Percentual de desconto
- Resultado com valor final e economia

## 💻 Como usar
1. Baixe os arquivos
2. Abra o `index.html` no seu navegador

## 🛠️ Tecnologias
- HTML
- CSS
- JavaScript
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Calculadora de Desconto</title>
</head>
<body>
    <h2>Calculadora de Desconto</h2>
    <label>Valor original: <input id="valor" type="number"></label><br>
    <label>Desconto (%): <input id="desconto" type="number"></label><br><br>
    <button onclick="calcular()">Calcular</button>

    <p id="resultado"></p>

    <script>
        function calcular() {
            const valor = parseFloat(document.getElementById('valor').value);
            const desconto = parseFloat(document.getElementById('desconto').value);

            const valorDesconto = valor * (desconto / 100);
            const valorFinal = valor - valorDesconto;

            document.getElementById('resultado').innerHTML =
                `Valor com desconto: R$ ${valorFinal.toFixed(2)}<br>
                 Você economizou: R$ ${valorDesconto.toFixed(2)}`;
        }
    </script>
</body>
</html>

---
Feito com 💙 por Juliana Ferreira

