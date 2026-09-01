# Regras de Negócio

## Visão geral

Este documento registra regras de negócio iniciais do MedTech Acessível.

As regras de negócio representam condições e restrições relacionadas ao domínio da gestão de equipamentos médico-hospitalares que deverão orientar o comportamento da plataforma.

Nesta etapa, as regras representam uma modelagem inicial e deverão ser revisadas conforme o domínio e os requisitos do sistema forem aprofundados.

---

## Equipamentos

### RN-01 — Identificação do equipamento

Cada equipamento cadastrado deverá possuir uma identificação que permita diferenciá-lo dos demais registros da instituição.

Os critérios definitivos de unicidade serão definidos durante a modelagem dos dados.

### RN-02 — Dados obrigatórios

O cadastro de um equipamento deverá possuir um conjunto mínimo de informações obrigatórias.

Os campos obrigatórios definitivos serão estabelecidos durante o refinamento dos requisitos.

### RN-03 — Situação operacional

Cada equipamento deverá possuir uma situação operacional válida entre as opções definidas pelo sistema.

As situações e suas possíveis transições serão especificadas posteriormente.

### RN-04 — Atualização cadastral

Somente usuários com permissão adequada poderão modificar informações cadastrais dos equipamentos.

---

## Intervenções

### RN-05 — Associação com equipamento

Toda intervenção registrada deverá estar associada a um equipamento existente na plataforma.

### RN-06 — Identificação da intervenção

Cada intervenção deverá possuir informações suficientes para identificar a atividade realizada e seu contexto.

### RN-07 — Tipo de intervenção

Cada intervenção deverá possuir uma classificação válida de acordo com os tipos definidos pelo sistema.

Entre os tipos inicialmente considerados estão:

- manutenção corretiva;
- manutenção preventiva;
- inspeção;
- calibração;
- outras atividades técnicas.

### RN-08 — Histórico

As intervenções registradas deverão compor o histórico do equipamento correspondente.

A estratégia para alteração, correção ou preservação de registros históricos será definida durante o refinamento das regras e dos requisitos de auditoria.

---

## Usuários e acesso

### RN-09 — Autenticação

O acesso às funcionalidades protegidas dependerá de autenticação válida.

### RN-10 — Permissões

As operações disponíveis poderão variar conforme as permissões associadas ao usuário.

Os perfis e níveis de acesso serão definidos em etapa posterior.

### RN-11 — Responsabilidade das operações

Quando tecnicamente e funcionalmente necessário, operações relevantes deverão permitir identificar o usuário responsável por sua realização.

---

## Integridade das informações

### RN-12 — Validação

O sistema deverá validar informações obrigatórias antes de concluir operações que dependam desses dados.

### RN-13 — Relacionamentos

Registros que dependam de outras entidades deverão preservar a integridade dos relacionamentos existentes.

### RN-14 — Exclusão de informações

A estratégia para exclusão de equipamentos, intervenções e outros registros deverá considerar a necessidade de preservação do histórico e da rastreabilidade.

A exclusão definitiva de informações não será assumida como comportamento padrão até que seus impactos sejam analisados.

---

## Evolução das regras

As regras de negócio deverão ser refinadas conforme:

- processos reais sejam analisados;
- usuários sejam consultados;
- requisitos sejam detalhados;
- o modelo de dados seja desenvolvido;
- questões de segurança e auditoria sejam avaliadas;
- novas funcionalidades sejam incorporadas.

As regras aqui apresentadas não constituem ainda uma especificação definitiva do domínio.
