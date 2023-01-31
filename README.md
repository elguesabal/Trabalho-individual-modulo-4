# Trabalho-individual-modulo-4


![diagrama modulo 4](https://user-images.githubusercontent.com/113626409/215622140-c9657de1-4b43-4b2b-86a9-846812e348ba.png)


Existem outras entidades além dessas três?
Sim, professor e salas são dois exemplos.


Quais são os principais campos e tipos?
Dentro de "Cursos" temos: "Nome do curso" (varchar) e "Disciplinas" (varchar).
Dentro de "Turmas" temos: "Nome da turma" (varchar) e "quantidade de alunos" (int).
Dentro de "Alunos" temos: "Matrícula" (varchar) e "Notas" (float).


Como essas entidades estão relacionadas?
Um curso pode ter várias turmas (0,n).
Uma turma pode ter somente um curso (0,1).
Uma turma tem muitos alunos (0,n).
Um aluno pode ter várias turmas (0,n).



Script para criar o banco de dados:

1- Código para ativar o mysql:
mysql -u root -p


2- Criar o banco de dados:
create database resilia;


3- Usar o banco de dados:
use resilia;


4- Criar a tabela:
create table cursos (
nome_do_curso varchar(10) primary key,
disciplinas varchar(10));

create table turmas (
nome_da_turma varchar(10) primary key,
quantidade_de_alunos int);

create table alunos (
matricula varchar(10) primary key,
notas int));


5- Visualizar as tabelas:
show tables;


6- Descrever a estrutura da tabela:
describe cursos;
describe turmas;
describe alunos;


#Veja abaixo na prática

![print1](https://user-images.githubusercontent.com/113626409/215624359-1039b8a3-8048-4026-a934-0f4e34c8182f.png)
![print2](https://user-images.githubusercontent.com/113626409/215624377-699fe89c-f2f9-4dd8-901b-5342feab7cf6.png)
