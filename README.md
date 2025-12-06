# 🤸‍♂️ Sistema de Pontuação de Ginástica Artística

Este projeto é uma aplicação em **JavaScript** desenvolvida para calcular a média final de notas de atletas em uma competição de ginástica artística. O sistema processa as notas atribuídas por cinco jurados, aplicando regras específicas de eliminação de notas extremas para garantir uma avaliação justa.

## 📋 Funcionalidades

O script realiza as seguintes operações para cada atleta listado:
1.  **Recebimento de Dados:** Lê uma matriz de objetos contendo o nome do atleta e suas 5 notas (de 0 a 10).
2.  **Ordenação:** Organiza as notas para identificar a maior e a menor.
3.  **Regra de Eliminação:** Descarta a maior e a menor nota (baseado no regulamento da competição).
4.  **Cálculo da Média:** Calcula a média aritmética das três notas centrais restantes.
5.  **Exibição:** Apresenta no console o nome do atleta, as notas originais ordenadas e a média final calculada.

## 🚀 Como Rodar o Projeto

Você pode executar este código de duas maneiras principais: utilizando o **Node.js** (recomendado) ou diretamente no **Console do Navegador**.

### Opção 1: Usando Node.js (Recomendado)

Certifique-se de ter o [Node.js](https://nodejs.org/) instalado em sua máquina.

1.  Clone este repositório ou baixe o arquivo do código.
2.  Salve o código JavaScript em um arquivo, por exemplo: `notas_atletas.js`.
3.  Abra o terminal na pasta onde o arquivo foi salvo.
4.  Execute o comando:

```bash
node notas_atletas.js
```

### Opção 2: Usando o Navegador (Chrome/Firefox/Edge)

Se você não tiver o Node.js instalado, pode rodar diretamente no navegador:

1.  Abra qualquer página da web.
2.  Aperte `F12` ou clique com o botão direito e selecione **Inspecionar**.
3.  Vá para a aba **Console**.
4.  Copie todo o código JavaScript e cole na área de digitação do console.
5.  Aperte `Enter` para ver o resultado.

## 🛠️ Tecnologias Utilizadas

* **JavaScript (ES6+)**: Linguagem principal utilizada para a lógica.
    * Métodos de Array: `.sort()`, `.slice()`, `.forEach()`, `.map()`.
    * Estruturas de Repetição: `for`.

## 🧮 Lógica do Cálculo

Para garantir a precisão conforme o enunciado:
1.  As notas são copiadas e ordenadas **numericamente** para garantir que a maior e menor nota real sejam identificadas.
2.  Utiliza-se `slice(1, 4)` para pegar apenas as três notas centrais.
3.  Para a exibição final (`Notas Obtidas`), as notas originais são ordenadas visualmente (formato texto) para atender aos requisitos de saída do desafio.

## 📄 Exemplo de Saída

Ao executar o script, o resultado no terminal será:

```text
Atleta: Cesar Abascal
Notas Obtidas: 10,10,7.88,8.42,9.34
Média Válida: 9.253333333333332

Atleta: Fernando Puntel
Notas Obtidas: 10,10,7,8,9.33
Média Válida: 9.11
Atleta: Daiane Jelinsky
Notas Obtidas: 10,7,8,9.5,9.5
Média Válida: 9

Atleta: Daiane Jelinsky
Notas Obtidas: 10,7,8,9.5,9.5
Média Válida: 9

Atleta: Bruno Castro
Notas Obtidas: 10,10,10,9,9.5
Média Válida: 9.833333333333334
```

---
