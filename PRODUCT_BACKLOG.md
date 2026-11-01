# Product Backlog - TaskEasy

> **Projeto:** TaskEasy — Gerenciador de Tarefas Simples  
> **Disciplina:** Requisitos de Software  
> **Etapa:** 1 — Product Backlog Inicial  
> **Versão:** 1.0

## Sumário

1. [Visão Geral](#1-visão-geral)
2. [Personas](#2-personas)
3. [Épicos](#3-épicos)
4. [Product Backlog](#4-product-backlog)
5. [Definition of Ready (DoR)](#5-definition-of-ready-dor)
6. [Definition of Done (DoD)](#6-definition-of-done-dod)
7. [Resumo de Prioridades](#7-resumo-de-prioridades)

---

## 1. Visão Geral

### Declaração do Problema

| | |
|:--|:--|
| **O problema de** | dificuldade para organizar e acompanhar tarefas do dia a dia |
| **Afeta** | estudantes e pessoas que precisam administrar atividades pessoais ou profissionais |
| **Cujo impacto é** | esquecimentos, atrasos e falta de clareza sobre atividades pendentes |
| **Uma boa solução seria** | um sistema simples para cadastrar, consultar, editar, excluir e concluir tarefas |

### Declaração do Produto

> Para pessoas que precisam organizar suas atividades, o **TaskEasy** é um gerenciador de tarefas simples que permite registrar atividades, definir prazos e acompanhar sua conclusão. Diferente de anotações dispersas, o sistema reúne as tarefas em uma única lista fácil de consultar.

---

## 2. Personas

| ID | Persona | Papel | Necessidade principal |
|:--|:--|:--|:--|
| P1 | Marina Costa | Estudante | Organizar trabalhos, estudos e prazos |
| P2 | Pedro Almeida | Trabalhador | Acompanhar tarefas profissionais e pessoais |

> Consulte os detalhes em [PERSONAS.md](./PERSONAS.md).

---

## 3. Épicos

| ID | Épico | Descrição |
|:--|:--|:--|
| EP01 | Cadastro e acesso | Permitir que o usuário crie uma conta e acesse o sistema |
| EP02 | Gerenciamento de tarefas | Cadastrar, visualizar, editar e excluir tarefas |
| EP03 | Acompanhamento | Marcar tarefas como concluídas e filtrar a lista |

---

## 4. Product Backlog

### Legenda de Prioridade (MoSCoW)

| Prioridade | Significado |
|:--|:--|
| **[MUST]** | Essencial para a primeira versão |
| **[SHOULD]** | Importante, mas não impede o funcionamento básico |
| **[COULD]** | Desejável, caso exista tempo |
| **[WONT]** | Fora do escopo desta versão |

### Legenda de Story Points (Fibonacci)

| SP | Tamanho |
|:--:|:--|
| 1 | Muito pequeno |
| 2–3 | Pequeno |
| 5 | Médio |
| 8 | Grande |

### EP01 — Cadastro e acesso

| ID | História de Usuário | Critérios de Aceitação | Prioridade | SP |
|:--|:--|:--|:--:|:--:|
| US01 | Como **visitante**, quero **criar uma conta** para utilizar o TaskEasy. | Formulário solicita nome, e-mail e senha; campos obrigatórios são validados; o sistema informa se o e-mail já estiver cadastrado. | [SHOULD] | 3 |
| US02 | Como **usuário cadastrado**, quero **entrar com meu e-mail e senha** para acessar minhas tarefas. | Deve existir formulário de login; dados incorretos exibem mensagem de erro; acesso é permitido somente com credenciais válidas. | [SHOULD] | 3 |
| US03 | Como **usuário**, quero **sair da minha conta** para encerrar meu acesso com segurança. | Deve existir opção de sair; após a ação, o usuário retorna à tela de login. | [COULD] | 1 |

### EP02 — Gerenciamento de tarefas

| ID | História de Usuário | Critérios de Aceitação | Prioridade | SP |
|:--|:--|:--|:--:|:--:|
| US04 | Como **usuário**, quero **cadastrar uma tarefa** para registrar uma atividade que preciso realizar. | Deve ser possível informar título e descrição; o título é obrigatório; após salvar, a tarefa aparece na lista. | [MUST] | 3 |
| US05 | Como **usuário**, quero **definir uma data de vencimento** para organizar minhas atividades por prazo. | Deve existir campo de data; a data escolhida deve aparecer nos detalhes da tarefa; o sistema não deve aceitar formato inválido. | [SHOULD] | 2 |
| US06 | Como **usuário**, quero **visualizar minhas tarefas** para saber quais atividades estão registradas. | A lista apresenta as tarefas cadastradas; cada item exibe título e situação; quando não houver tarefas, uma mensagem informativa é apresentada. | [MUST] | 3 |
| US07 | Como **usuário**, quero **editar uma tarefa** para corrigir ou atualizar suas informações. | Deve ser possível alterar título, descrição e data; as alterações são salvas; a lista apresenta os dados atualizados. | [MUST] | 3 |
| US08 | Como **usuário**, quero **excluir uma tarefa** para remover atividades que não preciso mais realizar. | Deve existir opção de exclusão; o sistema solicita confirmação; após confirmar, a tarefa deixa de aparecer na lista. | [MUST] | 2 |

### EP03 — Acompanhamento

| ID | História de Usuário | Critérios de Aceitação | Prioridade | SP |
|:--|:--|:--|:--:|:--:|
| US09 | Como **usuário**, quero **marcar uma tarefa como concluída** para registrar que finalizei a atividade. | Deve existir opção para concluir; a situação é atualizada; a tarefa continua disponível na lista como concluída. | [MUST] | 2 |
| US10 | Como **usuário**, quero **visualizar separadamente tarefas pendentes e concluídas** para acompanhar meu progresso. | Deve existir opção de filtro; o filtro pendente mostra apenas tarefas não concluídas; o filtro concluído mostra apenas tarefas finalizadas. | [SHOULD] | 3 |
| US11 | Como **usuário**, quero **ordenar tarefas pela data de vencimento** para visualizar primeiro as atividades com prazo mais próximo. | Deve existir opção de ordenação por data; tarefas com datas mais próximas aparecem primeiro; tarefas sem data ficam ao final. | [COULD] | 3 |
| US12 | Como **usuário**, quero **consultar a quantidade de tarefas pendentes e concluídas** para ter uma visão rápida do meu andamento. | O sistema apresenta a quantidade de tarefas em cada situação; os números são atualizados após cadastrar, concluir ou excluir uma tarefa. | [COULD] | 2 |

---

## 5. Definition of Ready (DoR)

Uma história de usuário está pronta para ser desenvolvida quando:

- [ ] Está escrita no formato "Como [persona], quero [ação] para [benefício]".
- [ ] Possui critérios de aceitação claros e verificáveis.
- [ ] Tem prioridade definida.
- [ ] Possui estimativa de Story Points.
- [ ] A equipe compreende o resultado esperado.
- [ ] Não possui dúvidas ou dependências que impeçam seu início.

---

## 6. Definition of Done (DoD)

Uma história de usuário está concluída quando:

- [ ] A funcionalidade foi implementada.
- [ ] Os critérios de aceitação foram verificados.
- [ ] Os principais cenários foram testados.
- [ ] Não existem erros conhecidos que impeçam seu uso.
- [ ] A alteração foi revisada pela equipe.
- [ ] A documentação foi atualizada, quando necessário.

---

## 7. Resumo de Prioridades

| Prioridade | Quantidade de histórias | Story Points |
|:--|:--:|:--:|
| [MUST] Must Have | 5 | 13 |
| [SHOULD] Should Have | 4 | 11 |
| [COULD] Could Have | 3 | 6 |
| [WONT] Won't Have | 0 | 0 |
| **Total** | **12** | **30** |

### Distribuição por Épico

| Épico | Must | Should | Could | Total de SP |
|:--|:--:|:--:|:--:|:--:|
| EP01 — Cadastro e acesso | 0 | 2 | 1 | 7 |
| EP02 — Gerenciamento de tarefas | 4 | 1 | 0 | 13 |
| EP03 — Acompanhamento | 1 | 1 | 2 | 10 |
| **Total** | **5** | **4** | **3** | **30** |

---

> **Observação:** este Product Backlog representa uma proposta inicial para a atividade acadêmica. As prioridades e estimativas podem ser revisadas pela equipe durante a discussão dos requisitos.
