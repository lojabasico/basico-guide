---
title: Configurar CWYP
---

# Configurar C.W.Y.P
Aqui será explicado o processo para fazer alteração de cor e descrição do texto das tiers de promoção de desconto.

___
## Cor das Tiers
O arquivo com as configurações de cores está localizado no Basico Theme:

basico-theme > src > assets > stylesheet > colors.scss

Para alterar a cor deve-se configurar aqui o valor da cor desejada:

{% codeblock %}
  $cwyp-color: #000;
{% endcodeblock %}

___
## Texto das Tiers
Para alterar o texto exibido junto com as tiers de desconto do produto, acessar:

basico-theme > src > assets > javascript > pages > product > components > attributes.js

Exemplo do código com as descrições dos preços.

{% codeblock %}
'discount_tier_info_mapping': [
          {
            'title': 'preço de custo',
            'description': 'este valor não cobre...
          },
        ]
{% endcodeblock %}

Exemplo da configuração de cor e descrição do texto que será exibido no site:

![](/images/config_cwyp/tiers_colors.png)
