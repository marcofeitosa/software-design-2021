## Desafio 4x4

[EnigMais](https://www.enigmais.com.br/) é uma empresa goiana que comercializa vários “desafios”. Um deles é o “quadrado mágico”. Nele você deve dispor todos os números inteiros naturais de 1 a 16em uma matriz 4x4 de tal forma que as somas dos números em cada uma das linhas, em cada uma das colunas e em cada uma das diagonais seja 34. Dependendo da sua curiosidade, você pode consultar informações adicionais sobre [quadrados mágicos](https://pt.wikipedia.org/wiki/Quadrado_m%C3%A1gico). **O objetivo aqui é identificar todas as possíveis soluções**. Na ilustração abaixo o “quadrado”, “matriz” ou “tabuleiro” está parcialmente preenchido, restando o acréscimo dos números 2, 3, 4, 6, 10, 12 e 13. Observe que este preenchimento parcial não é parte de uma solução, pois a linha contendo 14 e 9, o que perfaz 23, precisa nas duas outras posições de números cuja soma deve perfazer 11, o que não é possível com os números ainda não empregados.

![Quadrado mágico 4x4](/avaliacao2/4x4.png)

### Proposta de Solução

Para identificar todas as possíveis soluções, podemos utilizar o Método de Narayana-De la Hire (uma variação do Método de Euler), explicado na versão em inglês da página da Wikipedia sobre [quadrados mágicos](https://en.wikipedia.org/wiki/Magic_square), que permite encontrar mais variações para quadrados de ordem par ao se aproveitar do fato de que a soma de uma progressão aritmética com número par de termos é igual à soma dos dois termos simétricos opostos multiplicados pelo número total de termos. A partir disso, pode-se utilizar a técnica da programação dinâmica para poupar recursos computacionais na busca pelas soluções possíveis, assim como técnicas de computação paralela. Pela simplicidade da estrutura, se não do algoritmo, uma arquitetura monolítica seria suficiente para atender os requisitos do sistema.


