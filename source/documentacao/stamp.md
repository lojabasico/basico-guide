---
title: Selo
---

# Selo
Essa página explica o processo para alterar o Selo da Vitrine e também o Selo da Página do Produto.

___
## Selo da Vitrine
Para alterar o selo que é exibido na vitrine deve-se fazer o seguinte processo:

Acessar *Customize* > *Theme Settings* > *Collection*.

![](/images/stamp/collection.png)

A imagem abaixo exibe a área onde deve ser inserido o código HTML e CSS para configurar o Selo da Vitrine.

![](/images/stamp/html_selos_vitrine.png)

Exemplo do código HTML para o Selo da Vitrine:

{% codeblock %}
  <stamp tag="bf-relampago" :product="product">
    <img src="https://cdn.shopify.com/s/files/1/2316/0905/files/selo-produto_relampago.png">
  </stamp>
{% endcodeblock %}

Tag                   | Aplicação                                 
---------             | ---------      
<stamp                | Todo conteúdo deve estar dentro do *stamp*.                                
tag="bf-relampago"    | O produto precisa conter a tag para conseguir ser exibido.
:product="product">   | Dificilmente esse valor será alterado. Deve ser atribuído ao __product__.
\<img src="https://"> | Normalmente usamos imagens, mas pode ser outra coisa, como um código HTML.

&nbsp;
Exemplo do código CSS do Selo da Vitrine:

{% codeblock %}
  .collection3__stripes .bf-relampago.stamp {
    width: 44px;
    margin-top: 14px;
  }
{% endcodeblock %}

A classe *.collection3_stripes* é referente ao elemento pai do *stamp*. Deve ser atribuído para não sobrescrever o estilo do selo.

___
## Selo do Produto
Para alterar o selo que é exibido na página do produto deve-se fazer o processo:  

Acessar *Customize* > *Theme Settings* > *Product Page*.

![](/images/stamp/product_page.png)

A imagem abaixo exibe a área onde deve ser inserido o código HTML e CSS para configurar o Selo do Produto.

![](/images/stamp/html_selos_produto.png)

Exemplo do código HTML para o Selo do Produto:

{% codeblock %}
  <stamp tag="algodao-pima" product="page">
    <img src="https://cdn.shopify.com/s/files/1/2316/0905/files/selo-pima.png">
  </stamp>
{% endcodeblock %}

Tag                   | Aplicação                                 
---------             | ---------
<stamp                | Todo conteúdo deve estar dentro do *stamp*.                                         
tag="algodão-pima"    | O produto precisa conter a tag para conseguir ser exibido.
product="page">       | Nunca altera esse valor. Sempre deve ser atribuído ao __page__.
\<img src="https://"> | Normalmente usamos imagens, mas pode ser outra coisa, como um código HTML.

&nbsp;
Exemplo do código CSS do Selo da Página do Produto:

{% codeblock %}
  .galleries__wrapper .algodao-pima.stamp {
    position: absolute;
    top: 14px;
    z-index: 999;
  }
{% endcodeblock %}

A classe *.galleries__wrapper* é referente ao elemento pai do *stamp*. Deve ser atribuído para não sobrescrever o estilo do selo.
