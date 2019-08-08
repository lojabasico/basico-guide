---
title: Página de Documentação
---

# Página de documentação
Essa página explica como criar uma nova página utilizando o Hexo que utiliza a linguagem Markdown. Também será explicado o processo para registrar a página na sua rede.

___
## Arquivo .md
Inicie seu editor de códigos e crie um arquivo do tipo .md dentro do diretório que estiver trabalhando.

Assim como estou mostrando nesse exemplo: process.md

![](/images/process/arquivomd.png)

___
## Markdown
O arquivo do tipo .md é a extensão para os arquivos do Markdow que é uma ferramenta de conversão de text-to-HTML e com ele é possível fazer uma marcação de forma mais limpa que o HTML.

Você pode encontrar uma explicação sobre o Markdow e como utilizar os códigos acessando: [Markdow](https://blog.da2k.com.br/2015/02/08/aprenda-markdown/)

Veja um exemplo de como fica o código do tipo .md dessa página que estou criando:

{% codeblock %}
---
title: Página de Documentação
---

# Página de documentação
Essa página explica como criar uma nova página utilizando o hexo que utiliza a linguagem Markdown. Também será explicado o processo para registrar a página na sua rede.

___
## Arquivo .md
Inicie seu editor de códigos e crie um arquivo do tipo .md dentro do diretório que estiver trabalhando.

Assim como estou mostrando nesse exemplo: process.md

![](/images/process/arquivomd.png)
{% endcodeblock %}

___
## Navigation.yaml
Até agora fizemos a criação da página com o conteúdo, o próximo passo é linkar a página com o menu.

Para adicionar a sua página no menu, você deve acessar o arquivo navigation.yaml no seu editor de códigos e inserir o caminho do link, como no exemplo abaixo:

{% codeblock %}
{
  "text": "Marketing",
  "type": "label",
  "children": [
    {
    "text": "Landing Page",
    "type": "link",
    "path": "marketing/landing_page.html"
    },
  ]
},
{% endcodeblock %}

___
## Terminal
Para visualizar como sua página está ficando você deve abrir o terminal de comando:

![](/images/process/terminal.png)

e digitar:
{% codeblock %}
$ cd <nomedapasta>/<pasta>
{% endcodeblock %}

quando estiver dentro do diretório desejado no terminal, digitar: *hexo server*.
{% codeblock %}
$ hexo server
{% endcodeblock %}

Se tudo der certo o endereço do *localhost* será exibido como a imagem abaixo:

![](/images/process/localhost.png)

Basta copiar o endereço e colar na sua barra de navegação. Você vai visualizar sua página renderizada.

___
## Subindo os arquivos
Por fim, digite o comando abaixo no terminal para subir as modificações do site.
{% codeblock %}
$ hexo generate
{% endcodeblock %}
