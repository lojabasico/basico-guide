---
title: Blacklist Cep
---

# Blacklist
Nessa página será explicado o processo para registrar um CEP suspeito na Blacklist.

___
## Shopify Flow
É necessário acessar o site do [basico.com/admin](http://basico.com/admin).

Acessar: Apps > Shopify Flow

No Shopify Flow é só procurar por *Suspeita de Fraude* como na imagem abaixo:

![](/images/blacklist/suspeita_fraude.png)

___
## Sumário do Workflow
Essa seção exibe o sumário dos CEPS cadastrados como Suspeita de Fraude.

![](/images/blacklist/summary_workflow.png)

___
## Editar Workflow
Ainda na seção *Workflow Summary* basta acessar o botão *Edit Workflow*.

![](/images/blacklist/edit_workflow.png)

Na parte inferior da página é possível registrar um novo CEP acessando *Add condition*.

![](/images/blacklist/whats_next.png)

E depois selecionar *is equal to* para digitar o CEP.

![](/images/blacklist/add_conditions.png)

Adicionar uma ação em *Add action*, selecionar *Send email* e definir a ação conforme a imagem abaixo:

![](/images/blacklist/add_action.png)

Também deve adicionar a ação *Add order tags* e inserir a tag *suspeita-de-fraude*.

___
## Salvar Modificações
Após fazer as modificações, não esquecer de salvar o arquivo.

![](/images/blacklist/save.png)
