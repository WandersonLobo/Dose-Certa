# Acompanhamento de Tratamentos com Medicamentos

## Sobre o projeto

Este projeto propõe a modelagem de um banco de dados para um sistema de apoio à organização e ao acompanhamento de tratamentos com diversos medicamentos.

O sistema permite registrar pacientes, tratamentos, prescrições, medicamentos, doses, períodos de uso e horários indicados. Também prevê o registro de cada dose como tomada, esquecida ou adiada e a autorização de cuidadores para acompanharem essas informações.

O sistema organiza as orientações cadastradas pelo paciente. Ele não recomenda medicamentos, não altera doses ou prescrições e não substitui a avaliação de profissionais de saúde.

## Objetivo

Desenvolver a modelagem conceitual e relacional de um banco de dados que represente as informações necessárias para acompanhar tratamentos prescritos e o registro de doses.

## Instituição e curso

- **Instituição:** Universidade Federal do Cariri (UFCA)
- **Curso:** Bacharelado em Engenharia de Software
- **Disciplina:** Banco de Dados

## Integrantes

- Caio Oliveira
- Davi Henrique
- Wanderson Francisco


## Modelagem do banco de dados

A documentação da modelagem está em [`tp1/modelagem.md`](tp1/modelagem.md). Ela reúne os requisitos, o modelo Entidade-Relacionamento, o diagrama, o esquema relacional, as dependências funcionais, a normalização e exemplos de dados e consultas.

## Escopo

O projeto considera o cadastro e o acompanhamento de tratamentos com medicamentos prescritos. A modelagem deve representar os pacientes e seus tratamentos, os medicamentos associados às prescrições, os horários de uso, o histórico de doses e o acesso de cuidadores autorizados.

## Limites do sistema

- Não recomendar medicamentos.
- Não alterar prescrições nem doses.
- Não substituir a avaliação ou a orientação de profissionais de saúde.