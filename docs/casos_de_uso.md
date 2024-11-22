# Sumário
- [Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)
- [Documentação dos casos de uso](#documentação-dos-casos-de-uso)
  - [Enviar Orçamentos](#enviar-orçamentos)
  - [Visualizar Solicitações Pendentes](#visualizar-solicitações-pendentes)
  - [Visualizar Orçamentos Pendentes](#visualizar-orçamentos-pendentes)
  - [Enviar APR](#enviar-apr)
  - [Deliberar Orçamentos](#deliberar-orçamentos)
  - [Fazer o Custeio das Viagens](#fazer-o-custeio-das-viagens)
  - [Fazer o Fluxo de Caixa das Equipes](#fazer-o-fluxo-de-caixa-das-equipes)
  - [Gerenciar Fiscais de Campo](#gerenciar-fiscais-de-campo)
  - [Gerenciar Viaturas](#gerenciar-viaturas)
 



## Diagrama de Casos de Uso
![Diagrama UML de Casos de Uso](https://github.com/henrymatheus/gestao_equipes/blob/2dcbf9644dcc63a9a010574afa5cdb0a498709ae/docs/images/diagrama_de_casos_de_uso.jpg)


## Documentação dos Casos de Uso

### Página Inicial
### Protótipo da Página Inicial
![Página Inicial](https://github.com/henrymatheus/gestao_equipes/blob/ad0212bb73edd0c03aeb4b2a79185a13a87b48b5/docs/images/Fisc.png)
----------------------------------------------------------------------------------------------


### Enviar Orçamentos
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Fiscal de campo

#### Cenário principal
1. O sistema exibe os três formulários de <strong> orçamentos </strong> com as seguintes informações:
    - Gestor (campo somente leitura)
    - Lider (combobox)
    - Equipe (campo editável e obrigatório)
    - Local de trabalho (campo editável e obrigatório)
    - Data do pedido (autopreenchido com a data do envio do orçamento)
    - Placa (campo editável e obrigatório)
    - Hodometro (campo editável e obrigatório)
    - Fornecedor (campo editável e obrigatório)
    - Dados para pagamento (campo editável e obrigatório)
    - Produto / serviço (campo editável e obrigatório)
    - Quantidade (campo editável e obrigatório)
    - Preço por unidade (campo editável e obrigatório)
    - Preço total (campo editável e obrigatório)    /(campo autopreenchido)
    - Total geral (campo editável e obrigatório)    /(Campo autoprenchido)
    - Ação "Enviar"
2. O usuário informa a equipe.
3. O usuário informa o local de trabalho, que corresponde a um município.
4. O usuário escolhe um município de trabalho a partir de uma lista (combobox) com os nomes dos municípios do estado do Pará.
5. O usuário informa a placa da viatura.
6. O usuário informa o valor do Hodometro da viatura.
7. O usuário informa o nome do fornecedor.
8. O usuário informa a placa da viatura.
9. O usuário informa o valor que consta no Hodometro.
10. O usuário informa os dados para pagamento. (opcional?)
11. O usuário informa o nome dos produtos que constam no orçamento.
12. O usuário informa a quantidade de produtos.
13. O usuário seleciona a opção "Salvar".
14. O sitema salva os dados.


#### Cenário alternativo 
- Nenhum cenário alternativo identificado.

#### Demais requisitos
- O sistema não deve permitir a inclusão de orçamentos de um mesmo fornecedor.
- O sistema não deve permitir o envio de menos de três orçamentos.
- O campo "Preço Total" irá conter o resultado da multiplicação "Quantidade" * "Preço" por unidade.
- O campo "Total Geral" irá conter a soma de todos os valores da coluna "Preço Total".

#### Protótipo do Caso de Uso Enviar Orçamentos
![Enviar orçamentos](https://github.com/henrymatheus/gestao_equipes/blob/cd580fd9fcce77dbcb29dd12ec6324d5ecbe501d/docs/images/enviar_orcamentos.png)
----------------------------------------------------------------------------------------------
### Visualizar Solicitações Pendentes
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir a visualização de orçamentos pendentes para aprovação <br>
Ator: Fiscal de campo

#### Cenário principal
1. O sistema exibe o formulário "Solicitações pendentes" contendo as seguintes informações:
    - Filtro de Equipe (combobox, opcional)
    - Nome da equipe (campo somente leitura)
    - Nº de solicitações pendentes (campo somente leitura)
    - Ação "Visualizar"
   
#### Cenário alternativo
1. Não há solicitações pendentes.
2. O sistema exibe uma mensagem na tela informando que no momento não existem solicitações pendentes.

#### Demais requisitos
1. O filtro de equipe deverá dispor dos nomes das equipes, exemplo: EQ01, EQ02, EQ03,etc.


#### Protótipo do Caso de Uso Visualizar Solicitações Pendentes
![Visualizar-Solicitações](https://github.com/henrymatheus/gestao_equipes/blob/0946eb5df9576b81acacff5830896d1e290ff2a4/docs/images/visualizar_solicitacoes.png)








----------------------------------------------------------------------------------------------
### Visualizar Orçamentos Pendentes
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir a visualização dos orçamentos pendentes <br>
Ator: Fiscal de campo

#### Cenário principal
1. O sistema exibe o formulário "Orçamentos pendentes" contendo as seguintes informações:
    - Nome da equipe (campo somente leitura)
    - Três formulários de orçamento referentes à solicitação selecionada (campos somente leitura)
    - Tempo desde o envio dos orçamentos (somente leitura)
    - Ação "Aprovar"
  
#### Cenário alternativo
1. O presidente está logado e decide visualizar os orçamentos.
2. O sistema exibe um botão de aprovação ao lado ou abaixo de cada orçamento.

#### Demais requisitos
1. O tempo desde o envio dos orçamentos pode estar disponível na forma de um cronômetro, ou uma contagem de dias.


#### Protótipo do Caso de Uso Visualizar Status dos Orçamentos







----------------------------------------------------------------------------------------------
### Enviar APR
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Fiscal de campo

#### Cenário principal
1. O sistema exibe uma lista de todas as APRS separadas por equipe e por mês:
   - Lista de quipes (list box)
   - lista dos meses do ano que conterão as APRS (LISTBOX)

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Enviar APR



### Deliberar Orçamentos
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Presidente

#### Cenário principal
1. O sistema exibe os orçamentos.
2. Deverá a aparecer um botão "Aprovar" ao lado de cada orçamento.
3. O presidente clica em um dos botões, aprovando, assim, um dos orçamentos.
4. O sistema exibe uma tela de confirmação com dois botões ("Sim" e "Não"), perguntando se o usuário quer mesmo aprovar o orçamento.
5. O usuário pressiona o botão "Sim".
6. A janela de confirmação fecha e todos os botões de aprovação ficam desabilitados.
7. O orçamento aprovado fica em destaque, e o botão consta "Aprovado".
8. O orçamento aprovado é devidamente identificado no banco de dados.
9. A solicitação em questão é devidamente indentificada no banco de dados.

#### Cenário alternativo
1. O usuário pressiona o botão "Não" da janela de confirmação.
2. A página permanece sem alteração até a aprovação de algum dos orçamentos.
#### Demais requisitos
- O presidente pode aprovar apenas um orçamento.
- Ao aprovar um orçamento, os outros dois deverão ficar desabiblitados e o botão "Aprovar" deverá contar "Aprovado" e também ficar desabilitado.
#### Protótipo do Caso de Uso Deliberar Orçamentos


### Fazer o Custeio das Viagens
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Líder de equipe

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Fazer o Custeio das Viagens

### Fazer o Fluxo de Caixa das Equipes
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Líder de equipe

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Fazer o Fluxo de Caixa das Equipes

### Gerenciar Fiscais de Campo
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Admin?

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Gerenciar Fiscais de Campo

### Gerenciar Viaturas
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Admin?

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Gerenciar Viaturas



### Links úteis: 
- #### Sintaxe básica e formatação de README: https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

