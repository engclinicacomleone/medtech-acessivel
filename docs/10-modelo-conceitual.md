# Modelo Conceitual Inicial

## Visão geral

Este documento apresenta uma primeira identificação conceitual das principais entidades envolvidas no MedTech Acessível.

O objetivo desta etapa não é definir tabelas, banco de dados ou tecnologias específicas, mas compreender quais elementos do domínio precisarão ser representados pelo sistema e como eles poderão se relacionar.

O modelo será refinado durante os estudos de análise de sistemas, modelagem de dados e banco de dados.

---

## Entidade: Usuário

Representa uma pessoa autorizada a utilizar funcionalidades da plataforma.

### Possíveis atributos

- identificador;
- nome;
- e-mail;
- credencial de acesso;
- situação do usuário;
- perfil ou nível de acesso;
- data de criação.

A estrutura definitiva dependerá do modelo de autenticação e autorização adotado futuramente.

---

## Entidade: Equipamento

Representa um equipamento médico-hospitalar gerenciado pela plataforma.

### Possíveis atributos

- identificador;
- nome ou tipo do equipamento;
- fabricante;
- modelo;
- número de série;
- número patrimonial;
- localização;
- situação operacional;
- observações;
- data de cadastro.

Essa entidade deverá concentrar as informações necessárias para identificação e acompanhamento do equipamento.

---

## Entidade: Intervenção

Representa uma atividade técnica registrada no histórico de determinado equipamento.

### Possíveis atributos

- identificador;
- equipamento relacionado;
- tipo da intervenção;
- data;
- descrição;
- responsável;
- situação;
- observações;
- data de registro.

---

## Entidade: Tipo de Intervenção

Representa uma classificação utilizada para organizar as intervenções registradas.

### Exemplos iniciais

- manutenção corretiva;
- manutenção preventiva;
- inspeção;
- calibração;
- outras atividades técnicas.

A necessidade de representar essa classificação como entidade independente será avaliada durante a modelagem lógica do banco de dados.

---

# Relacionamentos conceituais

## Equipamento e Intervenção

Um equipamento poderá possuir várias intervenções registradas ao longo de seu ciclo de vida.

Cada intervenção deverá estar associada a um equipamento.

Conceitualmente:

> Equipamento 1 → N Intervenções

---

## Usuário e Intervenção

Uma intervenção poderá possuir associação com o usuário responsável por seu registro na plataforma.

Conceitualmente:

> Usuário 1 → N Intervenções registradas

Essa relação não significa necessariamente que o usuário que registrou a informação tenha sido o profissional que executou fisicamente a intervenção.

Essa distinção deverá ser avaliada durante o refinamento do modelo.

---

## Representação simplificada

```text
USUÁRIO
   |
   | registra
   v
INTERVENÇÃO
   |
   | pertence a
   v
EQUIPAMENTO
