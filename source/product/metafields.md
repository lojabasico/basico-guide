---
title: Custom Fields
---

# Custom Fields
São metadata, conhecidos também por metafields, esses são os campos adicionais do cadastro do produto, e em alguns casos obrigatórios para o cadastro de produto.

Para realizar o cadastro dos Custom Fields, basta clicar em ***More Actions*** na parte superior da página do produto no admin.

*Visualização no admin:*
![](/images/products/metafields.png)

Os Custom Fields são:

| Campo | Obrigatório |
|-|-|
| Nome do Produto no Site | sim |
| Descrição | sim |
| Cor | sim |
| Hexadecimal da Cor | sim |
| Textura da Cor | não |
| Gênero da peça | sim |
| Tabela de tamanho do Size-Chart | não |
| Texto adicional | não |
| Descritivo da tabela | não |
| Imagem de Size Chart | não |
| Materiais | - |
| Nome do Material | não |
| Cores Mestres | sim |
| NCM | sim |
| Importado ou nacional | sim |
| Complete o Look | - |
| Veste Também | - |
| Meta Description | - |
| Esconder aviso de ultimas peças | não |
| Descritivo para Embalagem extra | - |
| Imagem para widget de embalagem extra | - |
| Titulo para widget de embalagem extra | - |
| Esconder a cor do titulo do Produto? | não |
| Produtos Filhos | - |
| Marketplace | não |
| Promo 3 preços | não |


A seguir seguem as descrições individuais de cada campo:

___
## Nome do Produto
Esse é o nome do produto exibido na página de produto e nas vitrines.

*Visualização no site:*
![](/images/metafields/title.png)

___
## Descrição
É o texto que descreve o produto, em sua respectiva página e em alguns anuncios de nossas redes sociais.

*Visualização no site:*
![](/images/metafields/description.png)

Existe nesse campo uma opção de ***Desabilitar conversão de HTML***, que serve para restringir o resultado do campo somente para texto.

___
## Cor
Defini a cor do produto. É exibido na página de produto e usado em anuncios.

___
## Hexadecimal da Cor
Esse campo só é obrigatório para popular o quadrado de seleção de cor mostrado na página de produto. Caso o campo ***Textura da Cor*** seja preenchido esse campo será sobreescrito, mas isso não tira a sua obrigatoriedade.

*Visualização no site:*
![](/images/metafields/color.png)

___
## Textura da Cor
Esse campo opcional sobreescreve o campo anterior (***Hexadecimal***) com uma imagem de textura. Ele é usado quando queremos ilustrar um tecido listrado ou com textura.

*Visualização no site:*
![](/images/metafields/texture.png)

___
## Gênero da peça
É importante o cadastro do gênero da peça, para poder, além de categorizaro o produto, propiciar segmentações por gênero em nossos anuncios e no próprio site.

``[OBS] Esse campo não é exibido no site!``

___
## Tabela de tamanho
Embora esse campo não seja obrigatório para não quebrar a experiência do usuario em nosso site, ele é muito imoportante, porque é nele que cadastramos a tabela de medidas dos tamanhos desse produto.

*Visualização no site:*
![](/images/metafields/table_sizes.png)

**IMPORTANTE!**
Esse campo segue um padrão de cadastro que é primordial de ser seguido, segue:

{% codeblock %}
<table class="table table-bordered">
  <tbody>
    <tr>
      <th></th>
      <th>38</th>
      <th>40</th>
      <th>42</th>
      <th>44</th>
      <th>46</th>
      <th>48</th>
      <th nowrap="nowrap">variação *</th>
    </tr>
    <tr>
      <td>cintura&nbsp;</td>
      <td>41</td>
      <td>43</td>
      <td>45</td>
      <td>47</td>
      <td>49</td>
      <td>51</td>
      <td>±1</td>
    </tr>
    <tr>
      <td>entrepernas&nbsp;</td>
      <td>27</td>
      <td>27</td>
      <td>27</td>
      <td>27</td>
      <td>27</td>
      <td>27</td>
      <td>±1</td>
    </tr>
  </tbody>
</table>
{% endcodeblock %}

___
## Texto adicional
Esse é um campo opcional, que mostra um texto após a tabela de medidas do Size-chart.

___
## Descritivo da tabela
Esse é o campo de legenda da tabela de medidas. É outro campo que também não é "obrigatório", mas que complementa a tabela que foi cadastrada anteriormente.

*Visualização no site:*
![](/images/metafields/table_info.png)

**IMPORTANTE!**
Esse campo segue um padrão de cadastro que é primordial de ser seguido, segue:

{% codeblock %}
<div>
  <h3>1 cintura&nbsp;</h3>
  <p>medir a frente da peça na altura do cós</p>
  <h3>2 entrepernas&nbsp;</h3>
  <p>medir toda extensão da perna pela parte interna, à partir do gancho até o final da peça</p>
</div>
{% endcodeblock %}

___
## Imagem de Size Chart
É o terceiro campo que complementa os dois anteriores e figura a tabela de medidas. Também não é obrigatório.

*Visualização no site:*
![](/images/metafields/table_image.png)

___
## Materiais
É um campo que esta desativado no momento. Ele servia para descrever os materiais do produto.

``[OBS] Esse campo não é exibido no site!``

___
## Nome do Material
É outro campo não obrigatório, mas que é muito util para caracterizar o produto.

``[OBS] Esse campo não é exibido no site!``

___
## Cores Mestres
É o grupo de cores à qual aquela produto pertece, por exemplo, se a cor principal do produto é marinho então esse produto pertece ao grupo "azul".

*Visualização no site:*
![](/images/metafields/breadcrumb.png)

___
## NCM
Esse campo é obrigatório porque ele contempla informações fiscais sobre o produto.

``[OBS] Esse campo não é exibido no site!``

___
## Importado ou nacional
Esse campo é obrigatório porque ele contempla informações fiscais sobre o produto.

Devem seguir os seguintes valores:

| Valor | Correspondência |
| - | - |
| 0 | Nacional |
| 1 | Importado |

``[OBS] Esse campo não é exibido no site!``

___
## Complete o Look
É um campo que esta desativado no momento. Ele servia para dar opções de complemento ao produto.

``[OBS] Esse campo não é exibido no site!``

___
## Veste Também
É um campo que esta desativado no momento. Ele servia para dar opções de complemento ao produto.

``[OBS] Esse campo não é exibido no site!``

___
## Meta Description
É um campo que esta desativado no momento. Ele servia para sobreescrever a metatag da página de produto.

``[OBS] Esse campo não é exibido no site!``

___
## Esconder aviso...
Essa opção esconde o aviso da página que o tamanho selecionado só tem algumas peças sobrando no estoque.

*Visualização no site:*
![](/images/metafields/last_units.png)

___
## Descritivo Embalagem
É um campo que esta desativado no momento. Mostrava um texto na página descrevendo o tamanho da caixa desse produto.

``[OBS] Esse campo não é exibido no site!``

___
## Imagem para widget
É um campo que esta desativado no momento. Comlementava o campo anterior.

``[OBS] Esse campo não é exibido no site!``

___
## Titulo para widget
É um campo que esta desativado no momento. Comlementava os campos anteriores.

``[OBS] Esse campo não é exibido no site!``

___
## Esconder a cor
Uma funcionalidade implementada por conta de uma necessidade. Essa opção retira a cor do titulo do produto.

___
## Produtos Filhos
É um campo que esta desativado no momento.

``[OBS] Esse campo não é exibido no site!``

___
## Marketplace
São campos opcionais que eram utilizados nas APIs do Pinterest.

### Descrição Otimizada
Campo opicional que pertece aos dados servidos para o Pinterest.

``[OBS] Esse campo não é exibido no site!``

___
### Nome de Produto
Campo opicional que pertece aos dados servidos para o Pinterest.

``[OBS] Esse campo não é exibido no site!``

___
## Promo 3 preços
Os campos a seguir pertencem a mecânica da promoção de 3 preços. Esses campos só são utilizados e aparentes no site caso a promoção esteja ativada.

### Tiers de Desconto
Códigos que aplicam diferentes preços para o mesmo produto, ex.: CWYPD565EF, CWYP5CE2FE

___
### Disponibilidade dos Tiers de Preço
Habilita ou desabilita o preço aplicado no campo anterior, ex.: false,true,true

___
## Estoque Integrado
Campo para cadastro da referência do produto mãe em casos de [Estoque Integrado](integrated_stock.html).
