---
layout: default
title: User Stories
permalink: /user-stories
---

# User Stories

## Histórias dos usuários

### Origens

- Originárias do XP (Extreme Programing), em 1998
- Surgidas da alegação que, no jogo de planejamento, os clientes definiam o escopo como histórias de usuários, que são como casos de uso

### O que é uma história do usuário

- É uma requisição de funcionalidade sobre o ponto de vista do usuário
- É uma expressão negociável de uma necessidade
- É uma expressão de um incremento de software

### Para o que serve

- Histórias de usuários servem para descrever funcionalidades que serão valiosas para os usuários do software

### O que NÃO é um história do usuário

- Não é uma especificação funcional
- Não é para relatar um bug
- Não é um documento de definições técnicas
- Não é uma enunciação detalhada
- Não é um requisito
- Não é um contrato
- Não é algo para funcionar sem o P.O.

> Um Épico é uma história muito grande que deverá ser decomposta depois ou um conjunto de histórias que formam uma entrega de valor específica (não um agrupamento aleatório)

## Por que escrevemos histórias, não requisitos e especificações

### Do manifesto ágil

- Indivíduos e interação entre eles mais que processos e ferramentas
- Software em funcionamento mais que documentação abrangente
- ***Colaboração com o cliente mais que negociação de contratos***
- Responder a mudanças mais que seguir um plano

### Ou seja

- Qualquer um pode escrever
- Qualquer um pode entender a demanda
- Foca na entrega de valor
- Facilita a mudança de comportamento
- Descreve uma possibilidade, não uma solução

## Escrevendo histórias de usuário

### 3Cs

Componentes da história do usuário propostos por Ron Jeffries

- Cartão
- Conversação
- Confirmação

### Anatomia básica

- Declaração de valor
- Regras de negócio
- Critérios de aceitação

## Modelos de declaração de valor

### Modelo Connextra

Modelo tradicional criado na Connextra em 2001.

- *Como*
- *quero/preciso/necessito de <meta/desejo>*
- *pois/de modo que <benefício>*

### Variações do modelo Connextra

- Mike Cohn: *Como , eu quero <meta/desejo>*
- Chris Matts: *A fim de \<receber benefício> como um , eu quero <meta/desejo>*
- 5Ws: *Como , eu , porque*
- Capital One: *Como um , eu posso <ação com o sistema> para que <benefício externo>*

### Quando a história é uma pergunta

- O que queremos validar?
- O que esperamos saber?
- O quanto pensamos que é necessário investir?

### Job Stories

- *Quando <situação>,*
- *Eu quero que <motivação>,*
- *Então eu posso*

### Quando a história é para caracterizar uma mudança ou diferenciação

- *Diferente do <situação atual ou indesejada>,*
- *Como , eu quero/preciso que <situação desejada>*

### Quando há uma necessidade que não entrega valor, mas é necessários ser feito

- *Precisamos de ,*
- *pois*

## Requisitos básicos de uma boa história

### INVEST

Seis atributos para uma boa história, de Bill Wake

- Independente (Independent)
- Negociável (Negotiable)
- Possui valor (Valuable to users or customers)
- Estimável (Estimatable)
- Pequena (Small)
- Testável (Testable)

### Não seja genérico

Uma das grandes vantagens das histórias dos usuários é fazer com que os desenvolvedores entendam mais das motivações dos usuários e tenham maior empatia por eles.

Abordagens genéricas não contribuem para isso.

> Ex.: Como usuário, eu preciso de …
>
> A identificação do usuário deve servir como ponto para discussão:

#### Pense

- O que ele faria?
- Como ele faria?
- Qual abordagem se adapta melhor a esse perfil de usuário?

Um contexto genérico não irá prover nada de interessante para discussão e melhoria do produto. Somente será uma desculpa para o aumento descontrolado do escopo, baseado em vontades individuais ou opiniões de Hippos

Ao eliminar o usuário genérico e focar em perfis concretos, torna-se mais fácil selecionar o que realmente é importante ser entregue.

### Descreva quem são esses usuários

Descrever e explicar quem são esses usuários permite a discussão e um entendimento compartilhado das necessidades a serem atendidas.

### Avalie a zona de controle e a esfera de influência

Todo sistema tem 3 áreas (Dettmer, William):

- A **zona de controle** que inclui aquelas coisas no sistema que nós podemos mudar nós mesmos
- A **esfera de influência** que inclui atividades que nós podemos impactar, mas não podemos exercer controle sobre
- E o **ambiente externo** que inclui os elementos que não temos nenhuma influência

Em uma boa história do usuário, o motivo da necessidade do usuário deve estar na esfera de influência do time, enquanto o entregável (o que o usuário quer), deve estar na zona de controle do time. Isso é dependente de contexto, não existem parâmetros universais que irão definir o que está na zona de controle e o que está na esfera de influência.

> Ex.:
>
> Como gerente de vendas, eu preciso saber o número total de vendas por vendedor, pois assim posso calcular e submeter as comissões mensais para o RH da empresa

Boas histórias sempre carregam algum risco na sua implantação. Quando o risco parece nulo, devemos ser cautelosos…

## Erros de controle excessivo

### Histórias falsas

Aquelas que enunciam necessidades do time.

- Como desenvolvedor, eu preciso…
- Como P.O., eu quero…
- Como testador, eu preciso…

São histórias falsas pois **não são usuários… tanto a necessidade quanto a entrega estão na zona de controle do time**

### Micro-histórias

Aquelas que é difícil identificar os riscos, dado que são tão pequenas que não permitem ver isso. Não são problemáticas por si só, mas deve haver uma análise mais ampla dos impactos que podem ser gerados e dos problemas quando vistas de um conjunto maior.

Devem ser eliminadas em planejamentos de médio e longo prazo, ou agrupadas em histórias maiores.

### Histórias enganadoras

Descrevem uma solução, e não uma necessidade do usuário.

> Ex.:
>
> Como administrador do sistema, para poder acessar mais rapidamente a interface principal, preciso que as requisições de javascript sejam reduzidas e saneadas

## Erros de falta de controle

### Expectativa completamente irreal

Quando o entregável não está na zona de controle do time.

> Ex.:
>
> A empresa está criando um software para acompanhamento médico, porém não possui nenhum controle do hardware ou algum equipamento de apoio. Eis a história:
>
> Como enfermeira, preciso que os dados do paciente sejam atualizados automaticamente no prontuário após o uso do esfigmomanômetro digital, para assim evitar erros de digitação ou perda de informações.

### História não é completamente acionável pelos desenvolvedores

Há alguma dependência de pessoas externas e haverá dificuldade em acessar a informação ou demora no processo.

As histórias devem ser quebradas até se tornarem acionáveis, com impedimentos contornáveis ou tratáveis rapidamente.

## Histórias com prazo de expiração

Muitas histórias dependem de prazo e, mesmo quando não importantes, devem receber uma atenção especial:

- Funcionalidades devido a mudanças na lei
- Prazos acertados em contrato

Ao invés de um controle constante ou da inserção de histórias no meio da iteração, essas histórias devem conter sua data limite no enunciado e ser separada das demais. Assim devem ser analisadas no início de cada iteração para garantir o atendimento.

Permitir mudanças de escopo não pode significar ignorar os limites de tempo e trabalho existentes na equipe. Se o time ficar constantemente atendendo a emergências, o resto do trabalho sofre pela falta de atenção e concentração, gerando erros e débito técnico. A emergência deve ser evitada ao máximo, e devem ser diferenciadas de alarmes falsos e das ansiedades dos stakeholders.

## Critérios de aceitação

Servem para definir quando que uma história está realmente completa, quais os seus limites e detalhamento da necessidade enunciada.

Tipos de parâmetros a serem descritos nos critérios de aceitação:

- Usabilidade
- Funcionalidade
- Prevenção e erros
- Performance
- Testes de estresse

## Usando histórias para planejar

### Evite o inferno de centenas de histórias (Story card hell)

O backlog deve ser hierárquico para garantir uma visão completa do que está sendo entregue. Um backlog linear, somente com elementos do mesmo tamanho, ou não permite um planejamento preciso (pois os itens são muito grandes) ou não permite uma visão e entrega completa do valor (pois os itens são muito pequenos).

Metáfora do Jeff Paton com o jogo Asteroids: você precisa quebrar os asteróides grandes até deixá-los tão pequenos que um raio laser certeiro seja capaz de destruí-lo. Mas não pode sair fragmentando todos, senão fica impossível de navegar e manobrar. Tem que manter um bom número de asteróides medianos para saber o que vai vir e fragmentar aqueles que dá conta de eliminar de verdade.

Um backlog hierárquico permite manter o foco no planejado e ao memso tempo gerar mudanças quando necessário. Vários stakeholders podem discutir, com base na granularidade que lhes parece mais compreensível. As mudanças de caminho tornam-se mais gerenciáveis e com pacotes de valor mais compreensíveis.

Devemos evitar quebrar os itens em tamanhos menores até o momento que seja necessário adicionar mais informações específicas, antes de precisarmos começar a trabalhar nesses itens.

Um backlog hierárquico evita esconder os aumentos desnecessários de escopo, já que há clareza no conjunto final. Além disso, o tempo de gerenciamento do backlog diminui, dado que há manejo fino de poucos itens.

### Outras sugestões para escrever melhores histórias de usuário

- Escreva cedo a declaração de valor
- Deixe para detalhar posteriormente
- Detalhar excessivamente no início pode dar a uma impressão falsa de completudeMuitos detalhes podem inibir a conversa sobre o valor a ser entregue
- Evite escrever soluções
- Pense em mais de um stakeholder que pode tirar proveito da solução para a situação elencada. Isso abre oportunidade para quebrar a história depois
- Use figuras para explicar a história
- Escreva as dúvidas
- Foque na declaração do problema/necessidade do usuário ao invés do problema técnico

### Referências

- Writing Stories, Kane Mar: [http://s3.amazonaws.com/public.kanemar.com/writingstories.ppt](http://s3.amazonaws.com/public.kanemar.com/writingstories.ppt)
- User Stories Applied for Agile Software Development (Capítulo 2), Mike Cohn: [https://www.mountaingoatsoftware.com/uploads/articles/User-Stories-Applied-Mike-Cohn.pdf](https://www.mountaingoatsoftware.com/uploads/articles/User-Stories-Applied-Mike-Cohn.pdf)
- Fifty Quick Ideas To Improve Your User Stories, Gojko Adzic & David Evans
- User Stories Done Right, Jeff Sutherland
