# Sumário
- [Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)
- [Documentação dos casos de uso](#documentação-dos-casos-de-uso)
  - [Enviar Orçamentos](#enviar-orçamentos)
  - [Visualizar Status Dos Orçamentos](#visualizar-status-dos-orçamentos)
  - [Enviar APR](#enviar-apr)
  - [Caso 4](#sample-section)
  - [Caso 5](#sample-section)
  - [Caso 6](#sample-section)
 



## Diagrama de Casos de Uso
![Diagrama UML de Casos de Uso](https://github.com/henrymatheus/gestao_equipes/blob/0ae4ca1d0ed88de9f906ab3372656a58cf0ff3c7/docs/Diagrama%20de%20Casos%20de%20Uso.jpg)


## Documentação dos Casos de Uso

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
  - Data do pedido (campo editável e obrigatório)
  - Placa (campo editável e obrigatório)
  - Hodometro (campo editável e obrigatório)
  - Fornecedor (campo editável e obrigatório)
  - Dados para pagamento (campo editável e obrigatório)
  - Produto / serviço (campo editável e obrigatório)
  - Quantidade (campo editável e obrigatório)
  - Preço por unidade (campo editável e obrigatório)
  - Preço total (campo editável e obrigatório)
  - Total geral (campo editável e obrigatório)
  - Data do pedido (autopreenchido com a data do envio do orçamento)
  - Ação "Enviar"
2. O usuário informa a equipe e os fiscais.
3. O usuário informa o local de trabalho, que corresponde a um município.
(...)
x. O usuário seleciona a opção "Salvar"
x. O sitema salva os dados.

 

#### Cenário alternativo 
- Nenhum cenário alternativo identificado.

#### Demais requisitos
- O sistema não deve permitir a inclusão de orçamentos de um mesmo fornecedor.
- O sistema não deve permitir o envio de menos de três orçamentos.

#### Protótipo do Caso de Uso Enviar Orçamentos








### Visualizar Status Dos Orçamentos
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Fiscal de campo

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Visualizar Status dos Orçamentos


### Enviar APR
Especificação funcional do Caso de Uso <br>
Objetivo: Permitir o envio de orçamentos para deliberação <br>
Ator: Fiscal de campo

#### Cenário principal

#### Cenário alternativo

#### Demais requisitos

#### Protótipo do Caso de Uso Enviar APR

### Links úteis: 
- #### Sintaxe básica e formatação de README: https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

