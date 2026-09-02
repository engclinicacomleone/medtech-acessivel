# Acessibilidade e Inclusão Digital

## Visão geral

A acessibilidade é um dos princípios centrais do MedTech Acessível.

O conceito de acessibilidade adotado pelo projeto não se limita à interface para pessoas com deficiência. Ele também considera barreiras tecnológicas relacionadas à conectividade, desempenho dos dispositivos, infraestrutura disponível e nível de familiaridade dos usuários com sistemas digitais.

O objetivo é desenvolver progressivamente uma solução que possa ser utilizada pelo maior número possível de profissionais dentro do público-alvo proposto.

## Princípios de acessibilidade

O desenvolvimento da plataforma deverá considerar quatro dimensões principais:

1. acessibilidade da interface;
2. compatibilidade com diferentes dispositivos;
3. funcionamento adequado em condições tecnológicas limitadas;
4. simplicidade de utilização.

## Acessibilidade da interface

A interface deverá ser desenvolvida considerando boas práticas de acessibilidade digital e, progressivamente, as recomendações das Web Content Accessibility Guidelines (WCAG).

Entre os requisitos previstos estão:

- estrutura semântica adequada das páginas;
- navegação por teclado;
- identificação clara dos campos de formulário;
- textos alternativos para conteúdos visuais relevantes;
- contraste adequado entre texto e fundo;
- mensagens de erro compreensíveis;
- indicação textual de estados e informações importantes;
- hierarquia consistente de títulos;
- compatibilidade com tecnologias assistivas sempre que tecnicamente possível.

A acessibilidade deverá ser considerada durante o desenvolvimento das funcionalidades, e não apenas como uma adaptação posterior.

## Design responsivo

A plataforma deverá possuir interface responsiva, permitindo sua utilização em diferentes tamanhos de tela.

A aplicação deverá priorizar inicialmente o acesso por:

- computadores;
- notebooks;
- tablets;
- smartphones por meio do navegador.

A proposta inicial é utilizar uma aplicação web responsiva, evitando a necessidade de desenvolvimento imediato de aplicativos nativos para diferentes sistemas operacionais.

## Conectividade limitada

Parte do público potencial poderá atuar em ambientes com conexões instáveis ou de baixa velocidade.

Por esse motivo, o projeto deverá buscar:

- reduzir transferências desnecessárias de dados;
- evitar recursos visuais excessivamente pesados;
- otimizar o carregamento das páginas;
- reduzir dependências externas desnecessárias;
- fornecer feedback adequado durante operações que dependam de conexão.

Sempre que uma operação envolver o preenchimento ou envio de informações relevantes, o projeto deverá considerar mecanismos que reduzam o risco de perda do registro em situações de conexão instável.

Como possibilidade conceitual, poderão ser avaliados recursos como salvamento temporário local ou em rascunho e envio ou sincronização posterior quando a conexão estiver novamente disponível.

A estratégia técnica definitiva será definida em etapas futuras, considerando aspectos de segurança, integridade dos dados e arquitetura da aplicação.

## Compatibilidade com hardware

O MedTech Acessível deverá evitar, sempre que possível, requisitos computacionais excessivos para operações básicas.

A aplicação deverá priorizar tecnologias web amplamente suportadas e interfaces que não dependam de alto poder de processamento no dispositivo do usuário.

A compatibilidade mínima deverá ser definida e testada quando uma primeira versão funcional estiver disponível.

## Simplicidade operacional

A inclusão digital também depende da facilidade de compreensão do sistema.

Por isso, a experiência do usuário deverá priorizar:

- linguagem clara;
- menus objetivos;
- quantidade reduzida de etapas para operações frequentes;
- consistência entre telas;
- feedback visual das ações realizadas;
- prevenção de erros;
- mensagens compreensíveis quando erros ocorrerem.

O objetivo é reduzir a curva de aprendizagem necessária para utilização das funções essenciais.

## Requisitos iniciais de acessibilidade

Os seguintes requisitos deverão orientar as primeiras versões funcionais:

| ID | Requisito |
|---|---|
| AC-01 | A interface deverá permitir navegação utilizando teclado. |
| AC-02 | Campos de formulário deverão possuir identificação textual clara. |
| AC-03 | Informações relevantes não deverão depender exclusivamente de cores. |
| AC-04 | A aplicação deverá utilizar contraste adequado para conteúdos textuais. |
| AC-05 | A interface deverá adaptar-se a diferentes tamanhos de tela. |
| AC-06 | Imagens informativas deverão possuir alternativa textual quando aplicável. |
| AC-07 | Mensagens de erro deverão indicar claramente o problema identificado. |
| AC-08 | Operações frequentes deverão possuir fluxos simples e consistentes. |
| AC-09 | A aplicação deverá evitar recursos desnecessariamente pesados. |
| AC-10 | O desenvolvimento deverá considerar progressivamente as recomendações WCAG. |
| AC-11 | O sistema deverá considerar mecanismos para reduzir a perda de informações durante interrupções de conexão em operações de registro. |

## Validação futura

Os requisitos de acessibilidade deverão ser validados progressivamente por meio de testes.

Entre as estratégias previstas estão:

- testes de navegação por teclado;
- análise de contraste;
- testes de responsividade;
- utilização de ferramentas automatizadas de avaliação;
- testes com tecnologias assistivas;
- avaliação de desempenho em conexões limitadas;
- testes com usuários.

Ferramentas automatizadas deverão ser utilizadas como apoio, e não como substitutas da avaliação humana.

## Limitações atuais

O projeto encontra-se em fase de concepção e documentação.

Portanto, os requisitos apresentados representam objetivos de desenvolvimento e ainda não constituem evidência de conformidade da plataforma com WCAG ou qualquer outro padrão de acessibilidade.

A conformidade somente poderá ser avaliada adequadamente após a implementação e os testes das interfaces.

## Evolução

À medida que o projeto avançar, este documento deverá ser atualizado com:

- critérios específicos de conformidade;
- resultados de testes;
- problemas de acessibilidade encontrados;
- correções implementadas;
- decisões de design;
- evidências de validação.
