# Histórias de Usuário

## Visão geral

Este documento apresenta histórias de usuário iniciais do MedTech Acessível.

As histórias traduzem necessidades dos usuários em objetivos que poderão orientar a definição das funcionalidades, prototipação, desenvolvimento e testes da plataforma.

As histórias ainda representam hipóteses e deverão ser refinadas e validadas durante a evolução do projeto.

## Estrutura utilizada

As histórias seguem, de forma geral, o formato:

> Como [tipo de usuário], quero [objetivo] para [benefício esperado].

Cada história poderá possuir critérios de aceitação que auxiliem na definição das condições mínimas necessárias para considerar a funcionalidade atendida.

---

## HU-01 — Acessar a plataforma

**Como** usuário autorizado,  
**quero** acessar a plataforma utilizando minhas credenciais,  
**para** utilizar as funcionalidades disponíveis para meu perfil.

### Critérios de aceitação

- O usuário deve informar suas credenciais.
- Credenciais válidas devem permitir acesso à área protegida.
- Credenciais inválidas não devem permitir acesso.
- O sistema deve informar quando a autenticação não for realizada com sucesso.

**Requisitos relacionados:** RF-01

---

## HU-02 — Encerrar sessão

**Como** usuário autenticado,  
**quero** encerrar minha sessão,  
**para** impedir que outra pessoa utilize meu acesso no dispositivo.

### Critérios de aceitação

- Deve existir uma opção para encerramento da sessão.
- Após o encerramento, funcionalidades protegidas não devem permanecer acessíveis sem nova autenticação.

**Requisitos relacionados:** RF-02

---

## HU-03 — Cadastrar equipamento

**Como** profissional responsável pela gestão dos equipamentos,  
**quero** cadastrar um equipamento médico-hospitalar,  
**para** manter suas informações centralizadas na plataforma.

### Critérios de aceitação

- O sistema deve disponibilizar formulário para cadastro.
- Os campos obrigatórios devem ser identificados.
- O sistema deve validar os dados necessários antes de concluir o cadastro.
- Após cadastro válido, o equipamento deve ficar disponível para consulta.
- O usuário deve receber confirmação da operação.

**Requisitos relacionados:** RF-03

---

## HU-04 — Consultar equipamentos

**Como** profissional responsável pelo parque tecnológico,  
**quero** visualizar os equipamentos cadastrados,  
**para** consultar as informações disponíveis sobre os ativos gerenciados.

### Critérios de aceitação

- O sistema deve apresentar os equipamentos cadastrados.
- O usuário deve conseguir acessar os detalhes de um equipamento.
- A interface deve apresentar as informações de maneira organizada.

**Requisitos relacionados:** RF-04 e RF-06

---

## HU-05 — Pesquisar equipamento

**Como** profissional responsável pela gestão dos equipamentos,  
**quero** pesquisar equipamentos cadastrados,  
**para** localizar rapidamente o ativo que preciso consultar.

### Critérios de aceitação

- O sistema deve disponibilizar mecanismo de pesquisa.
- A pesquisa deve utilizar pelo menos um atributo disponível no cadastro.
- O sistema deve apresentar os registros correspondentes.
- Quando nenhum resultado for encontrado, o usuário deve receber uma informação clara.

**Requisitos relacionados:** RF-05

---

## HU-06 — Atualizar equipamento

**Como** usuário autorizado,  
**quero** atualizar as informações de um equipamento,  
**para** manter seu cadastro consistente com a situação atual.

### Critérios de aceitação

- O sistema deve permitir acessar a edição de um equipamento existente.
- Os dados atuais devem ser apresentados para edição.
- Alterações válidas devem poder ser salvas.
- O usuário deve receber confirmação após a atualização.

**Requisitos relacionados:** RF-07

---

## HU-07 — Registrar intervenção

**Como** profissional responsável pelo acompanhamento técnico,  
**quero** registrar uma intervenção realizada em um equipamento,  
**para** manter seu histórico técnico atualizado.

### Critérios de aceitação

- A intervenção deve estar associada a um equipamento.
- O sistema deve permitir registrar informações básicas da intervenção.
- Os campos obrigatórios devem ser validados.
- Após o registro, a intervenção deve integrar o histórico do equipamento.

**Requisitos relacionados:** RF-08 e RF-10

---

## HU-08 — Consultar histórico

**Como** profissional responsável pela gestão ou manutenção,  
**quero** consultar o histórico de intervenções de um equipamento,  
**para** compreender as atividades realizadas ao longo de seu ciclo de vida.

### Critérios de aceitação

- O histórico deve estar associado ao equipamento selecionado.
- As intervenções registradas devem estar disponíveis para consulta.
- As informações devem permitir identificar quando e qual intervenção foi realizada.

**Requisitos relacionados:** RF-09

---

## Evolução

Novas histórias serão adicionadas conforme:

- requisitos forem refinados;
- novas funcionalidades forem propostas;
- usuários reais forem consultados;
- protótipos forem avaliados;
- novas necessidades forem identificadas.

Os critérios de aceitação também deverão evoluir para condições mais específicas e testáveis conforme o desenvolvimento avance.
