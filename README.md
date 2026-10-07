# projetos_html
🌸 Sarah Canaã — Loja de Moda Feminina

Um site moderno e responsivo para uma loja de moda feminina chamada Sarah Canaã, desenvolvido utilizando HTML, CSS e JavaScript.

O projeto possui uma identidade visual moderna, com o rosa como uma das cores principais, combinando elementos sofisticados e um estilo inspirado em interfaces modernas de moda e cultura pop.

✨ Sobre o projeto

O site foi criado para apresentar os produtos da loja Sarah Canaã de maneira bonita, organizada e fácil de navegar.

A página possui diferentes categorias de produtos, permitindo que o cliente encontre rapidamente o que procura.

Categorias disponíveis

👗 Vestidos

👟 Tênis & Sandálias

👚 Camisas Femininas

👖 Shorts & Calças

Cada produto possui:

Foto real do produto

Nome

Categoria

Descrição

Preço

Botão de compra

Botão para favoritar

🎨 Design

O projeto utiliza uma identidade visual baseada principalmente em:

🌸 Rosa

🖤 Preto

🤍 Branco

🩷 Tons claros de rosa

✨ Tons de lilás e creme

O design foi desenvolvido para transmitir uma sensação de elegância, modernidade e personalidade.

Também foram utilizados efeitos como:

Animações ao passar o mouse

Efeito de transparência

Gradientes

Sombras

Bordas arredondadas

Efeito de zoom nas imagens

Botões animados

Banner promocional

Botão flutuante do WhatsApp

🛍️ Estrutura do site

O site é dividido nas seguintes partes:

1. Header

O cabeçalho possui:

Logo da Sarah Canaã

Menu de navegação

Botão de pesquisa

Botão de favoritos

O menu permite acessar diretamente as categorias da loja.

2. Hero

É a primeira seção que o visitante encontra ao entrar no site.

Ela apresenta:

"Vista sua melhor versão."

Também possui botões para:

Explorar a coleção

Ver categorias

Além disso, existe uma imagem de destaque relacionada à moda feminina.

3. Pesquisa de produtos

O site possui uma barra de pesquisa.

O usuário pode digitar o nome de uma peça e os produtos são filtrados automaticamente.

Por exemplo:

vestido


O site mostrará apenas produtos relacionados a vestidos.

4. Categorias

A seção de categorias apresenta quatro opções:

Vestidos
Tênis & Sandálias
Camisas
Shorts & Calças


Ao clicar em uma categoria, o usuário é levado diretamente para a seção correspondente.

5. Produtos

Cada categoria possui produtos apresentados em cards.

Um card possui aproximadamente esta estrutura:

┌─────────────────────────┐
│                         │
│       FOTO REAL         │
│                         │
│                    ♡    │
├─────────────────────────┤
│ VESTIDO                 │
│ Vestido Pink Sunset     │
│ Vestido midi...         │
│                         │
│ R$ 189,90           +   │
└─────────────────────────┘


As imagens são inseridas utilizando a tag HTML:

<img src="URL_DA_IMAGEM" alt="Descrição">

❤️ Favoritos

Cada produto possui um botão de coração.

Ao clicar nele:

♡ → ♥


O coração muda de aparência para indicar que o produto foi marcado como favorito.

Essa funcionalidade é feita com JavaScript.

🔎 Pesquisa

A pesquisa utiliza JavaScript para filtrar os produtos.

A função responsável por isso é:

function searchProducts() {
    ...
}


Ela verifica o texto digitado pelo usuário e compara com o conteúdo dos produtos.

💬 WhatsApp

O site possui integração com o WhatsApp.

Existe um botão flutuante no canto inferior direito da tela.

Também existem botões dentro do site que levam o cliente para o WhatsApp.

Quando o usuário seleciona um produto, uma mensagem pode ser criada automaticamente.

Por exemplo:

Olá! Tenho interesse no produto: Vestido Pink Sunset.
Gostaria de saber mais informações e consultar a disponibilidade.

📱 Responsividade

O site foi desenvolvido para funcionar em diferentes tamanhos de tela.

Ele possui regras CSS para:

💻 Computadores

💻 Notebooks

📱 Celulares

📱 Tablets

O CSS utiliza @media para adaptar o layout.

Exemplo:

@media(max-width: 600px) {
    .products {
        grid-template-columns: 1fr 1fr;
    }
}


Isso permite que os produtos se adaptem a telas menores.

🧰 Tecnologias utilizadas

O projeto foi desenvolvido utilizando:

HTML5

Responsável pela estrutura do site.

CSS3

Responsável por:

Cores

Layout

Responsividade

Animações

Gradientes

Tipografia

Efeitos visuais

JavaScript

Responsável pelas interações:

Pesquisa

Favoritos

WhatsApp

Botões dos produtos

Google Fonts

O projeto utiliza as fontes:

DM Sans

Playfair Display

📁 Estrutura do projeto

Atualmente, o projeto pode ser executado utilizando apenas um arquivo:

sarah-canaa/
│
└── index.html


O HTML contém:

HTML
├── Estrutura da página
├── CSS
└── JavaScript


Em uma versão futura, o projeto pode ser organizado da seguinte maneira:

sarah-canaa/
│
├── index.html
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
├── images/
│   ├── vestidos/
│   ├── calcados/
│   ├── camisas/
│   └── calcas/
│
└── README.md


Essa estrutura é recomendada para projetos maiores porque facilita a manutenção do código.

⚙️ Configurando o WhatsApp

No arquivo index.html, procure:

const whatsappNumber = "5511999999999";


Substitua pelo número de WhatsApp da loja.

Exemplo

Se o número for:

(11) 99999-9999


Utilize:

const whatsappNumber = "5511999999999";


Não utilize:

+
()
-
espaços


O número deve conter apenas os números.

🖼️ Alterando as imagens

Para alterar uma imagem de produto, procure por:

<img
    src="URL_DA_IMAGEM"
    alt="Nome do produto"
>


Substitua o endereço dentro de src.

Por exemplo:

<img
    src="images/vestido-rosa.jpg"
    alt="Vestido rosa"
>


Se você colocar suas próprias imagens no projeto, pode utilizar:

images/
├── vestido-rosa.jpg
├── vestido-preto.jpg
├── tenis-branco.jpg
└── camisa-rosa.jpg

💰 Alterando preços

Os preços podem ser alterados diretamente no HTML.

Exemplo:

<strong class="price">
    R$ 189,90
</strong>


Para mudar para R$ 199,90:

<strong class="price">
    R$ 199,90
</strong>

👗 Adicionando novos produtos

Para adicionar um novo produto, você pode copiar um dos elementos:

<article class="product">
    ...
</article>


E alterar:

Imagem

Nome

Categoria

Descrição

Preço

Produto enviado para o WhatsApp

Exemplo:

<article class="product">

    <div class="product-image pink">

        <button class="favorite">♡</button>

        <img
            src="images/novo-produto.jpg"
            alt="Novo produto"
        >

    </div>

    <div class="product-info">

        <span class="product-category">
            Vestido
        </span>

        <h3>Novo Vestido</h3>

        <p>Descrição do novo produto.</p>

        <div class="price-row">

            <strong class="price">
                R$ 199,90
            </strong>

            <button
                class="buy"
                onclick="buy('Novo Vestido')"
            >
                +
            </button>

        </div>

    </div>

</article>

🚀 Como executar

Não é necessário instalar nenhum programa ou biblioteca.

Basta:

Baixar ou clonar o projeto.

Abrir a pasta.

Abrir o arquivo index.html.

O site será carregado no navegador.

Também é possível utilizar extensões como Live Server no Visual Studio Code para visualizar o site durante o desenvolvimento.

🌐 Publicando o projeto

O projeto pode ser publicado gratuitamente utilizando serviços como:

GitHub Pages

Netlify

Vercel

Depois de publicado, o site poderá ser acessado através de um endereço na internet.

📌 Próximas melhorias

Algumas funcionalidades que podem ser adicionadas futuramente:

🛒 Carrinho de compras

💳 Sistema de pagamento

👤 Área do cliente

🔐 Login e cadastro

📦 Sistema de pedidos

📊 Painel administrativo

❤️ Lista de favoritos permanente

🔍 Filtros por tamanho e preço

🏷️ Sistema de cupons

📱 Menu mobile

🖼️ Galeria com várias fotos por produto

🌐 Domínio próprio

👩‍💻 Objetivo do projeto

O objetivo deste projeto é criar uma vitrine virtual moderna para a Sarah Canaã, apresentando os produtos de maneira visualmente atrativa e facilitando o contato entre a loja e seus clientes.

📄 Licença

Este projeto pode ser utilizado como base para estudos, portfólio e desenvolvimento de uma loja virtual.

As imagens utilizadas no projeto devem ser verificadas quanto às suas respectivas licenças antes de serem utilizadas comercialmente.

🌸 Sarah Canaã

Moda feminina para mulheres que transformam presença em estilo.

Vista sua melhor versão. 💗


Esse README já está estruturado para ficar bonito diretamente na página do **GitHub**, com título, emojis, explicação das tecnologias, estrutura de pastas, configuração do WhatsApp e instruções para modificar produtos.