# mod03_projeto_individual
Neste projeto foi proposto a criação de entidades relacionais que pudessem atender a regra de negócio da Resilia Data.

## Proposta:

Você foi contratado para desenvolver um banco de dados que irá armazenar dados
importantes que será utilizado pelo sistema RESILIADATA.
➔ O sistema irá auxiliar na avaliação de quais são as tecnologias que as empresas parceiras
estão utilizando e quem são seus colaboradores;
➔ Vamos ter o cadastro de empresas parceiras, cadastro de tecnologias com a opção de
selecionar a área (webdev, dados, marketing, etc.), uma tabela para registrar quais
tecnologias as empresas estão utilizando e uma tabela para cadastro de colaboradores.

## Solução:
- Criação de três tabelas simples que pudessem fazer uso
do relacionamento para complementar informações.

## Resposta das perguntas 
Realizar essa modelagem e responder algumas perguntas com nosso
modelo:

1. Quais são as entidades necessárias?

 -Foram necessárias pelo menos três entidades.

2. Quais são os principais campos e seus respectivos tipos?
 
 - empresas_parceiras: id_emp tipo inteiro.
 - colaboradores: id_colab tipo inteiro.
 - tecnologia: id_tec tipo inteiro.

3. Como essas entidades estão relacionadas?
 - Estão relaciionadas por meios de chave primária na tabela empresas_parceiras e chaves secundárias nas tabelas colaboradores e tecnologia.
 
4. Simule 2 registros para cada entidade.
 - Suponhamos que já temos um banco de dados e as tabelas criadas.
 -Registro01:
 	INSERT INTO colaboradores (
 	id_colab, 
 	empresa_id,
	username,
	funcao,
	setorvar,
	cel,
	tempo_empresa
	)
	VALUES (
	1345678,
	78945,
	"Alberto L.",
	"analista de mídias sociais",
 	"markerting",
 	"011988888888",
 	'01-03-2020'
 	);
 	
  - Registro02:
  	INSERT INTO tecnologia (
	id_tec,
	web_dev,
	id_empresadados,
	empresa,
	markerting,
	cnpj,
	status
	)
	VALUES(
	00014,
	00178,
	"Tecnology Company SA",
	"0001111000/0001-00",
	"Ativa"
  	);
  
