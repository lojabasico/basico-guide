---
title: Promos
---

# Promos ON/OFF
Essa página explica o processo que deve ser feito para ativar e desativar as promoções do site, por exemplo, 20% off na parte de baixo, 20% na segunda peça de linho e outras promoções existentes.

___
## Script Editor
Dentro dos **apps** do site existe um que se chama *Script Editor*.
Esse é um app padrão do Shopify e é usado justamente para alterar o script do carrinho do Shopify, possibilitando essas diferentes promos.

--- **IMPORTANTE!** ---
`Lembre-se de tomar muito cuidado ao mexer com isso, porque esse código afeta várias outras áreas e funcionalidades do site.`

![](/images/promo/script_editor.png)

Porém existe uma limitação nesse app. Ele só consegue executar um script por vez.

**Não é possível habilitar mais de um script em PROD.**

___
## Várias Promos Simultâneas

Por causa desse motivo de não poder rodar mais de um script ao mesmo tempo, foi desenvolvido um padrão para escrever as promos em formato de classe e chama-las simultaneamente dentro de um único script.

Após acessar o app *Script Editor* procurar pelo script **Várias Promos Simultâneas**.

![](/images/promo/promo_simultanea.png)

Será o único script com status **Published**.

___
## Editando o Script

Para poder editar o script é necessário despublica-lo primeiro. Lembre-se que não pode deixar despublicado por muito tempo.

Para despublicar é só clicar no botão do lado direito em cima:

![](/images/promo/unpublish.png)

Depois de despublicar, você vai ver que tem uma aba com **Input e Code**. Essa aba por padrão fica em Input, onde mostra um campo para inserir produtos de teste no carrinho de teste desse app:

![](/images/promo/code_input.png)

Para editar o script basta clicar em **Code**.

___
## Configurando a Promo

![](/images/promo/config_promo.png)

Esse objeto é o objeto de configuração da promo de Linho.

Essa promo aplica um desconto de 2 em 2 produtos (pode-se mudar isso alterando a variável *discount_per_n_products*) que tenham a tag da var *categoryx* (no caso da imagem é linho) e aplica 10% de desconto (variável *discount*).

Se quiser aplicar mais ou menos desconto nos produtos, lembre-se que a variável *discount* é multiplicada pelo valor original do produto, por isso ela é 0.90, para aplicar 10%.

No caso:

+ 10% - 0.90
+ 20% - 0.80
+ 30% - 0.70

___
## Ativando a Promo
Depois de configurada, é preciso adicionar a promo dentro do array que vai para o método run da classe PromoMachine, como mostra a imagem:

![](/images/promo/promo_machine.png)

--- **IMPORTANTE!** ---
`Para desativar essa ou qualquer outra promo, é só tirar ela desse array.`

Depois de colocar ela no array, o script vai dar uma processada (canto direito de cima).

Se tudo estiver certo vai ficar assim:

![](/images/promo/script_status.png)

Pode-se testar a promo na aba input, procurando produtos que tenham a tag e incluindo eles.

Depois, clicando em Run Script (do lado direito em cima) para ver se ele aplica o desconto, mas isso é opcional.

___
## Publicando
Por fim é só clicar no botão *Save and Publish* e pronto!

![](/images/promo/save_publish.png)

___
## Desligando
Apenas para reforçar essa etapa.

Na etapa *ativando a promo*, onde foi editado o código e adicionado a promo no array do método run, basta tirar dali e deixar todo o resto como esta para desativar a promoção.

![](/images/promo/promo_off.png)
