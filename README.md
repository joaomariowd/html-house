# Tutorial de HTML

##  Alterar cores dos elementos da casa

### Arquivo de CSS principal

```shell
user@machine:~$ css/style.css
```

## Itens (classes) da casa

- Chaminé: .chimney
- Degraus: .doorsteps
- Janelas: .window
  - Detalhe: .sash
- Paredes: .wall
- Teto: .roof
  - Detalhe: .dormer
- Porta: .door
  - Maçaneta: .handle

## Objetivo

Deixar o desenho bem colorido.

Fazer vários experimentos. Pode-se mexer nas classes mais genéricas, tipo ```.window```, que irá alterar todas as janelas.

Porém, para customizar apenas a janela da porta, por exemplo, alterar a classe ```.door .window```.

Também é possível alterar propriedades como largura ```width```, altura ```height```, que no exemplo estão definidas em percentagens.

## Inspetor

Abrir o inspetor, clicando com o botão direito do mouse no elemento que se quer inspecionar e em seguida clicar em  Inspecionar.

Todas as propriedades podem ser alteradas pelo Inspetor, para testes.

### Exemplo

Clicando com o botão direito no teto e em seguida Inspecionar, abrirá o Inspetor focado no teto. 

Do lado direito aparece as propriedades de ```.house .roof```.

Alterando a cor da propriedade ```border-top:``` de *black* para *red*, podemos ver como ficaria o teto vermelho.

Em seguida, *recarregar a página* apertando F5 ou na 'seta redonda' no cabeçalho do navegador, verifica-se que ao recarregar a página os valores voltam aos originais.

Ao alterar as propriedades pelo inspetor, os valores não ficam gravados.

No teto, bem como outros elementos pode-se mexer também nos valores em pixels (unidade px) ou percentagens (%) para alterar os tamanhos desses elementos.

## Enfim, o céu é o limite. Queremos ver essa casa colorida e diferente da original ;)))

## Desafio

Um degrau de cada cor!

Descobrir qual classe única de cada degrau e customizar a cor de fundo para cada uma.

Dica: utilizar o inspetor para descobrir as classes únicas de cada degrau.

Dica 2: se o seletor para essas classes únicas não existir no arquivo style.css, abrir um seletor novo para cada classe.

## Curiosidade sobre o Inspetor

Na aba **Styles** ele mostra todas as regras de CSS aplicadas a cada elemento.

Na aba **Computed** aparece os valores que foram de fato aplicados a cada elemento.

As regras de CSS mais genéricas são substituidas pelas mais específicas sucessivamente.

**Exemplo**: Alterando a cor de fundo da janela ```.window```, será alterado em todas as janelas. 

Ajustando o elemento ```.door .window``` a cor da janela da porta ficará diferente das demais.