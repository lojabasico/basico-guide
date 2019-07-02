---
title: Novo Produto
---

# Novo Produto
Segue o processo de cadastro de um novo produto na plataforma do basico.com (Shopify).

## Pré Requisitos
Antes de cadastrar um produto na plataforma, é crucial ter o material referente ao produto pronto para ser cadastrado préviamente. O nome do produto deve estar definido e as fotos referentes devem estar tratadas.

## Shopify
Na aba produtos existe um botão (canto direito superior) que leva para a página de cadastro do novo produto.

![](/images/products/addButtom.png)

Nessa página temos campos que são usados para diferentes funcionalidades do sistema.

![](/images/products/page.png)

___

## Campos

Seguindo o cadastro, existem campos do sistema obrigatórios, campos de sistema opcionais e custom fields. A seguir listamos os campos do cadastro explicando suas funcionalidades individualmente:

| Campo | Obrigatório | Utilização |
|-|-|-|
| Title | sim | admin |
| Description | não | página de produto |
| Images | sim | página de produto, vitrines, anuncios |
| Pricing | não | - |
| Inventory | não | - |
| Shipping | não | - |
| Variants | sim | página de produto, vitrines, anuncios |
| Search engine listing preview | não | admin, página de produto |
| Product availability | não | página de produto, vitrines |
| Product Type | sim | página de produto, vitrines, anuncios |
| Vendor | sim | página de produto |
| Collections | não | vitrines |
| Tags | não | vitrines, anuncios |
| Theme templates | não | página de produto |

Além dos desses campos que são o ***core*** do cadastro existem ainda os [Custom Fields](/metafields) que também são obrigatórios no cadastro de produto.

A seguir seguem as descrições individuais de cada campo:

___
### Title
Esse campo é o nome programatico do produto. É usado para que o produto seja encontrado no sistema, pelo pessoal do Picking e também no app de POS (iPad das lojas). Por essas razões esse campo é obrigatório no cadastro de produtos.

Esse campo é usado inicialmente para gerar handle do produto. Mas uma vez que o produto é criado (primeira vez que é salvo) ele não altera mais o handle do produto.

``[OBS] Esse campo não é exibido no site!``

___
### Description
Esse campo é usado para popular com HTML a página do produto no site. Ele é usado somente no caso de uma customização individual (somente para o produto que o campo tiver valor editado), caso contrário é recomendado que deixe esse campo em branco para que a página de produto siga com a configuração default do site.

*Visualização no site (configuração default do site):*
![](/images/products/[page]description.png)

___
### Images
Aqui é onde são cadastradas as imagens do novo produto. Essas imagens são usadas tanto na página de produto, como nas vitrines e também em alguns de nossos anuncios em redes sociais.

*Visualização no admin:*
![](/images/products/images.png)

*Visualização no site:*
![](/images/products/[page]images.png)

___
### Pricing
Esse campo não é utilizado e pode ser deixado em branco, porque o cadastro de produtos utiliza o sistema de variants que será descrito mais adiante.

``[OBS] Esse campo não é exibido no site!``

___
### Inventory
Esse campo não é utilizado e pode ser deixado em branco, porque o cadastro de produtos utiliza o sistema de variants que será descrito mais adiante.

``[OBS] Esse campo não é exibido no site!``

___
### Shipping
Esse campo não é utilizado e pode ser deixado em branco, porque o cadastro de produtos utiliza o sistema de variants que será descrito mais adiante.

``[OBS] Esse campo não é exibido no site!``

___
### Variants
Aqui é importante ter em mente que é onde serão cadastrados todos os campos anteriores (estoque, preço e tamanhos). A primeira coisa a ser feita é setar a primeira (e unica) opção que utilizamos no site: tamanho (escrita em português mesmo!)

*Visualização no admin:*
![](/images/products/variants.png)

Os valores são os respectivos tamanhos do produto, ex.: pp, p, m, g e gg.

Após setar os diferentes tamanhos é possivel cadastrar os outros campos individualmente por variant, são eles:

- Price
- SKU
- Quantity (aqui devemos acrescentar a quantidade do estoque por localidade)

*Visualização no admin:*
![](/images/products/inside_variant.png)

___
### Search engine listing preview
Esse campo é preenchido automaticamente, mas pode ser editado para uma possivel customização do handle do produto. Aqui também é possivel criar um link de redirect desse mesmo produto.

Além do handle são cadastrados o titulo e a descrição da página (HTML).

*Visualização no admin:*
![](/images/products/handle.png)

___
### Product availability
Esse painel é o primeiro do lado esquerdo da página de cadastro de produto. Ele serve para publicar ou despublicar o produto do site, nos diferentes canais que temos cadastrados:

| Campo | Canal | Utilização |
|-|-|-|
| Online Store | site | sim |
| Point of Sale | iPads das lojas | sim |
| Mobile App | celular | sim |
| Buy Button | app do shopify | não |
| Instagram | app do shopify | não |
| Shopify CLI | app do shopify | não |

A seleção desses canais publicam ou despublicam o produtos em seus respectivos.
___
### Organization
Aqui cadastramos 2 informações cruciais para o produto, o *Product Type* e o *Vendor*. Existem mais dois campos nesse painel que são *Collections* e *Tags*, mas ambom são preenchidos automaticamente, porem é possível ao cadastrar um novo produto querer adicionar tags customizadas, confira essas tags na página das [Tags](tags).

*Visualização no admin:*
![](/images/products/vendor.png)

**Product Type:** Aqui definimos o tipo do produto, ex.: Camisetas, Vestidos, Calças, etc.
Esse campo é importante porque ele é usado para categorizar os produtos em suas respectivas vitrines.

**Vendor**: Esse campo é usado para definir produtos do mesmo tipo que tem cores diferentes, ex.: camiseta gola c masculina

___
### Theme templates
Esse campo altera o template da página de produto. Ele é usado somente pela T.I. em casos específicos e não deve ser alterado.

___
### Metafields || Custom Fields
Após salvar o cadastro dos campos citados anteriormente, devemos cadastrar os [Custom Fields](/metafields).

*Visualização no admin:*
![](/images/products/metafields.png)
