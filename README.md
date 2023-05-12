# Media Queries com CSS

[Clique aqui para acessar o site](https://filipe-bacof.github.io/Media-Queries-CSS/)

Para quem quiser o degradê utilizado, aqui está:
```
linear-gradient(45deg, #405de6, #5851db, #833ab4, #c13584, #e1306c, #fd1d1d)
```

## Como aplicar estilizações para diferentes tamanhos de tela
- Uma media query é um recurso do CSS3 que faz com que uma página da web se adapte a tamanhos de tela e tipos de mídia diferentes.
- Dentro das **CONDIÇÕES** abaixo, podemos passar vários tipos de regras:
```
@media (CONDIÇÕES) {
    #id {
        color: red;
    }
    .classe {
        color: green;
    }
    elemento {
        color: blue;
    }
}
```
- Por Exemplo, se a tela possuir no máximo 1000px de largura, podemos definir este `breakpoint` nas condições:
```
@media (max-width: 1000px){ }
```
- Uma aplicação útil é o tamanho de fonte para telas menores:
```
body {
  font-size: 2rem;
}

@media (max-width: 500px) {
  body {
    font-size: 1.5rem;
  }
}
```
- Nesse caso, o tamanho de fonte será alterado para telas de no máximo 500px
### Lembrando que:
`1rem = 16px` | `1.5rem = 24px` | `2rem = 32px`

## Importante: Uma boa prática é que sempre coloque suas media queries no final do arquivo CSS.

# Tipos de mídia
Há muitos tipos de dispositivos, mas podemos agrupá-los em 4 categorias:

- `all` - todos os tipos de mídia (por padrão);
- `print` - para impressoras;
- `screen` - para telas de dispositivos;
- `speech` - para leitores de tela;

É possível concatenar regras, conforme abaixo utilizando a palavra **AND**:
```
@media screen and (max-width: 500px) { }
```

# Principais Breakpoints
- menor que 319: telas muito pequenas;
- 320px até 480px: dispositivos móveis;
- 481px até 768px: tablets e iPads;
- 769px até 1024px: laptops e telas pequenas;
- 1025px até 1200px: desktops, telas grandes;
- maior que 1201px: telas muito grandes, TVs;

# Sobre o Projeto
Neste projeto, utilizei as media queries para definir a largura das telas e adaptar a exibição de conteúdo em diferentes dispositivos, como celulares, tablets e computadores. Com isso, foi possível mostrar ou esconder a classe com um texto e uma imagem, facilitando o entendimento sobre responsividade e tamanhos de telas padrão.

Para complementar a experiência do usuário, incluí um degradê de cores no fundo do layout, inspirado na estética utilizada pelo Instagram. A ideia é fornecer um exemplo prático de como as media queries podem ser utilizadas para aprimorar a interface do usuário e criar layouts mais dinâmicos e atraentes. Espero que este projeto possa ajudar outros desenvolvedores que buscam entender melhor o uso das media queries em seus próprios projetos.

Nos dias atuais, o design responsivo é um elemento indispensável no desenvolvimento e design para web. As media queries desempenham um papel crucial na criação de layouts responsivos e adaptáveis a diferentes dispositivos. Espero que este texto tenha contribuído para o seu entendimento sobre o funcionamento das media queries e como utilizá-las em seus projetos de design e desenvolvimento web.
