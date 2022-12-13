# dda-lib-ads-SAP-Connector
Transações do SAP contendo as tabelas utilizadas para extrações do SAP Connector

Dicionário de transações / bases identificadas em testes de Receita, Compras, Lançamento Contábeis, Usuários, Depreciação e Ativos.

# Acelerador: Script ACL para extração de Boletos via SAP Connector


Atualizado por: Raul Moutinho
Última Versão: 01-12-2022

## 1-	Descrição
Script modelo para efetuar a extração dos Boletos registrados no SAP utilizando a ferramenta de SAP Connector via ACL.

## 2-	Pré Requisitos

Para adicionar o script a um ACL, é necessário que seja configurado o ACL para fazer a conexão juntamente com ajustes no próprio Script:

1)	Configurar o SAP Connector de acordo com o SAP do cliente
2)	Caminho da bibliotéca: "C:\Windows\System32\gsskrb5.dll"

## 3-	Passo a Passo

1)	Importar o script no ACL
2)	Configurar o SAP Connector
3)	Alterar o CAMINHO do script
4)	Alterar o partnername=p: para o configurado no SAP Connector
5)	Alterar o período de acordo com o necessário, "FEBKO"."AZDAT" BETWEEN 20210101 AND 20210101.
6)	Caso necessário, adicionar filtros de Empresa, ou o que for necessário.
7)  Executar o Script.


# Acelerador: Script ACL para extração dos Lançamentos de Retenção via SAP Connector


Atualizado por: Raul Moutinho
Última Versão: 01-12-2022

## 1-	Descrição
Script modelo para efetuar a extração dos Lançamentos de Retenção registrados no SAP utilizando a ferramenta de SAP Connector via ACL.

## 2-	Pré Requisitos

Para adicionar o script a um ACL, é necessário que seja configurado o ACL para fazer a conexão juntamente com ajustes no próprio Script:

1)	Configurar o SAP Connector de acordo com o SAP do cliente
2)	Caminho da bibliotéca: "C:\Windows\System32\gsskrb5.dll"

## 3-	Passo a Passo

1)	Importar o script no ACL
2)	Configurar o SAP Connector
3)	Alterar o CAMINHO do script
4)	Alterar o partnername=p: para o configurado no SAP Connector
5)	Alterar o período de acordo com o necessário: "WITH_ITEM"."AUGDT" BETWEEN 20201230 AND 20210531
6)	Alterar o ano de acordo com o período analisado: AND "WITH_ITEM"."GJAHR" = '2021'
7)	Caso necessário, adicionar filtros de Empresa, ou o que for necessário.
8)  Executar o Script.
