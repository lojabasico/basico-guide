---
title: Estoque Integrado
---

# Estoque Integrado
Segue o processo de cadastro de produtos com estoque integrado.

O estoque integrado consiste em *pelo menos* 2 cadastros de produto. Um produto conteria o estoque e o(s) outro(s) conteriam todas as outras informações.

A principal funcionalidade dessa integração é poder centralizar, organizar e conseguir controlar o estoque de peças que são vendidas para diferentes gêneros, por exemplo: **boyfriend**

___
## Produto Mãe (Feeder)
O produto mãe (**feeder**) é o produto onde será cadastrado o estoque. O procedimento de cadastro é o mesmo do [cadastro](new_prouduct.html) de produto comum, mas não é necessário cadastrar nenhum metafield para esse produto, e é de suma importancia não esquecer de cadastrar as tags para ocultar esse tipo de produto nas vitrines, página de busca e catálogos de anuncio das redes sociais (*hide_from_collection*, *hide_from_search* e  *hide_from_catalog*).  
É **primordial** que o produto mãe contenha as mesmas variants do produto filho com SKU cadastrado. O preço do produto mãe precisa estar certo, já que ele é usado nos produtos filhos.  

*Visualização no admin:*
![](/images/stock/variants.png)

--- **IMPORTANTE!** ---
`Não esquecer de cadastrar as tags:`
- hide_from_collection
- hide_from_search
- hide_from_catalog

*Obs.:* Não é aconselhavel a duplicação de produtos já existentes para o cadastro de *produtos mãe*, mas não deve quebrar a experiência caso isso seja feito.

___
## Produto Filho
O produto filho é cadastrado normalmente também, mas com uma peculiaridade, ele deve ter pelo menos 1 de quantidade em cada variant (tamanho) para que ele seja tagueado corretamente.

*Visualização no admin:*
![](/images/stock/variants.png)

Esse produto também precisa ter todos os metafields preenchidos e no final deve ser cadastrado a referencia ao seu produto mãe respectivo, no campo de **Estoque Integrado**.

*Visualização no admin:*
![](/images/stock/field.png)
