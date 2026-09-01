# Requisitos do Sistema

## Visão geral

Este documento registra os requisitos iniciais do MedTech Acessível.

Os requisitos representam comportamentos, funcionalidades e características esperadas da plataforma e serão refinados progressivamente conforme o projeto avance para etapas de modelagem, prototipação, desenvolvimento e validação.

Nesta fase, os requisitos são considerados hipóteses iniciais derivadas do problema, do público-alvo e da solução proposta.

## Tipos de requisitos

Os requisitos do projeto serão inicialmente classificados em duas categorias:

### Requisitos Funcionais (RF)

Descrevem funcionalidades e comportamentos que o sistema deverá oferecer aos usuários.

Em outras palavras, representam principalmente **o que o sistema deverá fazer**.

### Requisitos Não Funcionais (RNF)

Descrevem características, restrições e critérios de qualidade relacionados ao funcionamento da solução.

Podem envolver aspectos como:

- segurança;
- acessibilidade;
- desempenho;
- usabilidade;
- compatibilidade;
- disponibilidade;
- manutenção.

---

# Requisitos Funcionais

## Gestão de usuários

### RF-01 — Autenticação

O sistema deverá permitir que usuários autorizados realizem autenticação para acessar funcionalidades protegidas da plataforma.

### RF-02 — Encerramento de sessão

O sistema deverá permitir que o usuário autenticado encerre sua sessão.

---

## Gestão de equipamentos

### RF-03 — Cadastro de equipamento

O sistema deverá permitir o cadastro de equipamentos médico-hospitalares.

O cadastro poderá conter informações como:

- identificação;
- fabricante;
- modelo;
- número de série;
- número patrimonial;
- localização;
- situação operacional;
- observações.

### RF-04 — Consulta de equipamentos

O sistema deverá permitir a visualização dos equipamentos cadastrados.

### RF-05 — Pesquisa de equipamentos

O sistema deverá permitir a pesquisa de equipamentos utilizando critérios disponíveis no cadastro.

### RF-06 — Visualização individual

O sistema deverá permitir visualizar os detalhes de um equipamento específico.

### RF-07 — Edição de equipamento

O sistema deverá permitir a atualização das informações de equipamentos cadastrados por usuários autorizados.

---

## Gestão de intervenções

### RF-08 — Registro de intervenção

O sistema deverá permitir registrar uma intervenção associada a determinado equipamento.

O registro poderá conter informações como:

- tipo da intervenção;
- data;
- descrição;
- responsável;
- situação;
- observações.

### RF-09 — Histórico de intervenções

O sistema deverá permitir consultar o histórico de intervenções associadas a um equipamento.

### RF-10 — Tipos de intervenção

O sistema deverá permitir identificar diferentes categorias de intervenção, como:

- manutenção corretiva;
- manutenção preventiva;
- inspeção;
- calibração;
- outras atividades técnicas.

---

## Informações gerenciais

### RF-11 — Resumo do parque tecnológico

O sistema deverá apresentar informações resumidas sobre os equipamentos cadastrados.

### RF-12 — Indicadores básicos

O sistema deverá permitir a visualização de indicadores básicos derivados dos dados registrados na plataforma.

Os indicadores específicos serão definidos durante etapas posteriores do projeto.

---

# Requisitos Não Funcionais

## Acessibilidade

### RNF-01 — Navegação por teclado

As principais funcionalidades da interface deverão ser operáveis utilizando teclado.

### RNF-02 — Responsividade

A interface deverá adaptar-se a diferentes tamanhos de tela.

### RNF-03 — Informação independente de cor

Informações essenciais não deverão depender exclusivamente de cores para serem compreendidas.

### RNF-04 — Estrutura acessível

A interface deverá utilizar estrutura semântica adequada e considerar progressivamente as recomendações WCAG.

---

## Usabilidade

### RNF-05 — Clareza da interface

A interface deverá utilizar linguagem clara e organização consistente das informações.

### RNF-06 — Feedback das operações

O sistema deverá informar ao usuário o resultado das principais operações realizadas.

### RNF-07 — Tratamento de erros

Mensagens de erro deverão apresentar informações compreensíveis que auxiliem o usuário a identificar o problema ocorrido.

---

## Desempenho

### RNF-08 — Eficiência

A aplicação deverá evitar processamento e transferência de dados desnecessários durante operações comuns.

### RNF-09 — Conectividade limitada

A solução deverá considerar utilização em ambientes com conexões de internet limitadas ou instáveis.

Critérios mensuráveis de desempenho serão definidos após a implementação inicial.

---

## Segurança

### RNF-10 — Controle de acesso

Funcionalidades protegidas deverão estar disponíveis somente para usuários devidamente autenticados e autorizados.

### RNF-11 — Proteção das credenciais

Credenciais de autenticação não deverão ser armazenadas em texto simples.

### RNF-12 — Proteção das informações

A arquitetura deverá considerar mecanismos adequados para preservar confidencialidade, integridade e disponibilidade das informações conforme sua classificação e finalidade.

---

## Compatibilidade

### RNF-13 — Aplicação web

A primeira versão deverá ser desenvolvida como aplicação web.

### RNF-14 — Compatibilidade entre dispositivos

A plataforma deverá permitir utilização por computadores, notebooks, tablets e smartphones por meio de navegadores compatíveis.

---

## Manutenibilidade

### RNF-15 — Organização do código

O código-fonte deverá possuir estrutura organizada que facilite compreensão, manutenção e evolução.

### RNF-16 — Documentação

Decisões técnicas relevantes deverão ser documentadas no repositório.

---

# Priorização inicial

Nem todos os requisitos serão implementados simultaneamente.

Para uma primeira versão funcional, a prioridade inicial será:

| Prioridade | Requisitos |
|---|---|
| Essencial | RF-01, RF-02, RF-03, RF-04, RF-05, RF-06, RF-07, RF-08, RF-09 |
| Posterior | RF-10, RF-11, RF-12 |

Os requisitos não funcionais deverão ser considerados durante todo o processo de desenvolvimento e refinados conforme seja possível estabelecer critérios mensuráveis.

## Rastreabilidade

Cada requisito possui um identificador único.

Exemplo:

`RF-03 — Cadastro de equipamento`

Esse identificador poderá futuramente ser utilizado para relacionar:

- requisitos;
- histórias de usuário;
- casos de uso;
- protótipos;
- código;
- testes;
- documentação.

Essa relação permitirá acompanhar como cada necessidade do projeto evolui desde sua definição até sua implementação e validação.

## Estado atual

Os requisitos apresentados neste documento ainda não representam uma especificação definitiva do sistema.

Eles deverão ser revisados conforme:

- novos conhecimentos técnicos sejam adquiridos;
- usuários sejam consultados;
- protótipos sejam avaliados;
- regras de negócio sejam identificadas;
- limitações técnicas sejam descobertas;
- versões funcionais sejam desenvolvidas.

O levantamento de requisitos será, portanto, um processo contínuo durante a evolução do MedTech Acessível.
