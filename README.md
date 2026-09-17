# Alura Plus

Página de divulgação do **Alura+**, desenvolvida como exercício prático durante os estudos de HTML e CSS na [Alura](https://www.alura.com.br). O objetivo do projeto é reproduzir uma landing page de um serviço de assinatura de cursos, colocando em prática a estruturação semântica de conteúdo, a organização de estilos e a construção de layouts com CSS Grid e Flexbox.

## Acesse o projeto

A página está publicada em duas plataformas diferentes e pode ser acessada por qualquer um dos links abaixo, já que ambos exibem o mesmo site.

**Vercel:** [aluraplus-mu-eight-99.vercel.app](https://aluraplus-mu-eight-99.vercel.app)

**GitHub Pages:** [erikvks.github.io/aluraplus](https://erikvks.github.io/aluraplus/)

## Sobre a página

A página apresenta o Combo+, que une o Alura+ e o Alura Língua em uma única assinatura. Ela começa com uma seção principal contendo o título da oferta, a imagem do combo, os botões de assinatura e um aviso sobre preços. Em seguida vêm três seções que alternam imagem e texto, destacando que o conteúdo pode ser assistido em qualquer tela, que o combo reúne as duas plataformas e que os cursos podem ser baixados para ver sem internet. Depois há uma seção com os dispositivos compatíveis (TV, computadores, celulares e tablets) e, por fim, um rodapé com o logo, links institucionais e as informações legais do serviço.

## Estrutura de arquivos

```
alura-plus/
├── index.html
├── styles.css
└── img/
    ├── Background.png
    ├── Combo.png
    ├── Plataformas.png
    ├── Telas.png
    ├── Notebook.png
    ├── tv.png
    ├── computador.png
    ├── celular.png
    └── Logo.png
```

## O que foi aprendido

### HTML semântico

A página foi organizada com tags que descrevem o papel de cada parte do conteúdo, como `section` para os blocos temáticos, `footer` para o rodapé e `ul` com `li` para agrupar itens relacionados, como os dispositivos e os links do rodapé. Os títulos seguem uma hierarquia com `h1` para a chamada principal e `h2` para os subtítulos das seções. Todas as imagens receberam o atributo `alt`, o que melhora a acessibilidade para quem usa leitores de tela.

### Metodologia BEM

As classes seguem o padrão BEM (Bloco, Elemento, Modificador), que deixa claro a qual componente cada estilo pertence. Um exemplo é `container__caixa__titulo`, em que `container` é o bloco, `caixa` é um elemento dentro dele e `titulo` é um elemento da caixa. Classes como `botao_secundario` e `secundario` funcionam como variações que reaproveitam estilos já existentes e alteram apenas o necessário.

### Variáveis CSS

As cores e a fonte principal ficam centralizadas no seletor `:root` por meio de propriedades customizadas, como `--botao-azul` e `--cor-de-fundo`. Assim, para mudar a identidade visual da página basta alterar o valor em um único lugar, em vez de procurar cada ocorrência no arquivo.

### Reset e fonte externa

O seletor universal `*` zera as margens e espaçamentos padrão do navegador, garantindo um ponto de partida consistente. A fonte Inter é importada do Google Fonts com `@import` e aplicada a todo o `body`.

### Layout com Grid e Flexbox

A classe `.container` usa `display: grid` com duas colunas de 50% cada e altura de `100vh`, fazendo com que cada seção ocupe a tela inteira e fique dividida entre imagem e texto. Já a lista de dispositivos e a lista de links do rodapé usam `display: flex` com `justify-content: center` para alinhar os itens lado a lado, e o rodapé usa `gap` para espaçar os links de maneira uniforme.

### Imagem de fundo

A seção principal recebe uma imagem de fundo com `background-image`, configurada com `background-repeat: no-repeat` para não se repetir e `background-size: contain` para se ajustar ao espaço disponível.

### Links estilizados como botões

Os links de assinatura recebem cor de fundo, borda arredondada, espaçamento interno e `display: block`, passando a se comportar visualmente como botões. O botão secundário tem fundo transparente e apenas uma borda branca, criando uma hierarquia visual entre a ação principal e a alternativa.

### Pseudoclasses

As pseudoclasses `:hover` e `:active` dão retorno visual à interação do usuário. Os botões mudam de cor ao passar o mouse e os links do rodapé ficam azuis no hover e roxos no momento do clique.

## Como executar

Não é necessária nenhuma instalação. Basta clonar ou baixar o repositório e abrir o arquivo `index.html` no navegador, mantendo a pasta `img` no mesmo diretório para que as imagens sejam carregadas.

```bash
git clone <url-do-repositorio>
cd alura-plus
```

## Tecnologias

HTML5, CSS3 e Google Fonts (Inter).

## Créditos

Projeto desenvolvido durante um curso da [Alura](https://www.alura.com.br). O layout e as marcas Alura, Alura+ e Alura Língua pertencem à Alura.
