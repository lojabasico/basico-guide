---
title: Tags
---

# Tags
As tags no Shopify, podem ser aplicadas em quase todas as entidades de conteudo do CMS (produto, pedido, customer, etc). Nessa sessão vamos abordar somente as tags referente à produto.

As tags de produto são, em sua maior parte, cadastradas automaticamente por um app do Shopify o [SmartTags](https://apps.shopify.com/smart-tags?locale=pt-BR).

Em resumo, esse app lê os dados do produto cadastrado e automaticamente cadastra as respectivas tags.

Um produto cadastrado corretamente deve conter várias tags, para poder ser categorizado e ativar ou desativar suas respectivas mecânicas.

___
## Tamanho
Essas tags são cadastradas automaticamente segunindo o titulo das variants cadastradas no produto, ex.:

| Variant | Tag |
| - | - |
| **tamanho:** pp | pp |
| **tamanho:** p | p |
| **tamanho:** m | m |
| **tamanho:** g | g |
| **tamanho:** gg | gg |

___
## Gênero
As tags de gênero são cadastradas automaticamente pelo app e dependem do SKU das variant do respectivo produto, por exemplo:

![](/images/tags/gender.png)

O produto acima será preenchido com as seguintes tags:

- masculino
- masculina
- para-ele
- para-todos (tag genérica de gênero)
- homem

___
## Product Type
O campo ***Product Type*** também é salvo como tag automaticamente pelo app. Isso é feito porque muitas vitrines se baseiam em tags para selecionar os produtos automaticamente, ex.:

![](/images/tags/product_type.png)

___
## Kits
A tag ***kitable*** serve para ativar a funcionalidade de kits dos produtos. Essa tag não é adicionada automaticamente.

*Visualização no site:*
![](/images/tags/kitable.png)

___
## Esconder o Produto
Existem algumas tags que são colocadas manualmente nos produtos para esconde-los tanto no site (vitrines e resultado de busca) como nos anuncios das redes sociais.

| Tag | Funcionalidade |
| - | - |
| hide_from_collection | esconde das vitrines |
| hide_from_search | esconde o produto da página de busca |
| hide_from_catalog | esconde o produto dos catálogos de anuncios |

--- **IMPORTANTE!** ---
`Essas tags servem somente para esconder os produtos, isso não significa que eles estejam despublicados do sistema.`

___
## Material
Existem também tags referentes ao material do produto (ex.: algodao, pima, algodao-pima) que são cadastradas manualmente para poder filtrar os produtos em diferentes vitrines.

___
## Cores
Existem também tags referentes à cor do produto (ex.: branco, preto, marinho) que são cadastradas manualmente para poder filtrar os produtos em diferentes vitrines.

___
## Promoção
Existem tags que são cadastradas manualmente para habilitar o produto, para que o mesmo possa participar de mecanicas de promoção, ex.: **promo-top**, **natal**

___
## Editar Diversas Tags
Esse processo pode ser útil quando for necessário adicionar ou remover tags em diversos produtos ao mesmo tempo.

Acessar: Products

E procurar pelos produtos que deseja alterar. Pode-se selecionar todos produtos de uma vez e executar uma ação em *Actions*.

Adicionando tags *Add tags* ou removendo *Remove tags* conforme sua necessidade.

![](/images/tags/search_tag.png)

Basta adicionar uma tag nova ou alguma tag que já existe. Aplicar as mudanças em *Aplly changes*

![](/images/tags/add_tags.png)

Para consultar se a tag foi adicionada ou removida com sucesso, basta clicar no produto e verificar quais tags estão ativas no produto.

![](/images/tags/view_tags.png)

Aqui também é possível adicionar ou remover a tag em um único produto.
