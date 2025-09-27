# 📚 BookSync: Gerencie Suas Leituras com Facilidade

**BookSync** é uma plataforma digital **gratuita** e **multiplataforma** desenvolvida para ser um **organizador de leituras**. O projeto visa atender **leitores** que encontram dificuldade em **organizar e catalogar suas leituras**, oferecendo uma ferramenta prática para registrar, avaliar e gerenciar seu histórico de livros lidos e em andamento.

Diferente de redes sociais literárias como o Skoob, BookSync foca na organização e gestão pessoal, e **não é uma rede social**, nem loja virtual de livros, evitando desviar o foco do usuário da leitura.

---

## 💡 Contexto do Projeto e Metodologia

Este projeto foi desenvolvido como entrega do módulo de Gestão Ágil de Projetos e Produtos, aplicando os conhecimentos de **Lean Inception** para definição do **MVP (Produto Mínimo Viável)** e a criação de um **Backlog Emergente** detalhado no **Jira**.

### Público-Alvo (Persona Segmentada no MVP)

O **MVP (Minimum Viable Product)** inicial do BookSync é focado na persona **"A Leitora"**, uma Analista de Marketing Digital de 29 anos. Ela busca uma plataforma **simples, com design amigável e usabilidade**, que permita o registro rápido e intuitivo de suas leituras e status.

### Visão do Produto (Product Vision)

| Item | Descrição | Fonte |
| :--- | :--- | :--- |
| **For** (Para) | leitores | Lean Inception |
| **Whose** (Que têm) | dificuldade de organizar e catalogar suas leituras | Lean Inception |
| **The** (O produto) | BookSync, uma multiplataforma | Lean Inception |
| **That** (Que) | facilita a organização dos livros lidos | Lean Inception |
| **Different From** (Diferente de) | Skoob | Lean Inception |
| **Our Product** (Nosso produto) | não é uma rede social, evitando que você se desfoque da leitura | Lean Inception |

---

## 👨‍💻 Equipe Scrum Enxuta

O projeto BookSync é executado por uma equipe **Scrum enxuta** e **multifuncional**, contendo o mínimo necessário para entregar um MVP com qualidade:

| Papel | Foco no Projeto |
| :--- | :--- |
| **Product Owner (PO)** | Visão de produto, priorização do Backlog, comunicação com stakeholders. (Ex: Claudia Maia, Relatora dos Tickets Jira) |
| **Scrum Master (SM)** | Facilitação, remoção de impedimentos, garantia da metodologia. |
| **Desenvolvedor Full Stack** | Implementação de Backend (Flask), Frontend (SPA), Infraestrutura (Docker), Testes e Integração com APIs (Google Books). |

---

## 🎯 MVP e Backlog da Sprint 1

O **MVP (Produto Mínimo Viável)** proposto tem como principal objetivo **facilitar a gestão, o registro e a avaliação inicial de leituras**.

### Funcionalidades do MVP (Features)

1.  **Acesso e Segurança**: Cadastro e Login de usuário.
2.  **Busca de Livros**: Busca e Adição de livros via Google Books API.
3.  **Dashboard e Gestão**: Visualização da lista de livros e alteração de status (lendo, lido).
4.  **Avaliação**: Adicionar nota e comentário a um livro.

### Definition of Ready (DoR)

Para que uma História de Usuário (HU) possa ser levada para a Sprint, ela deve atender aos seguintes critérios:

* História descrita e priorizada no backlog.
* Critérios de aceitação definidos e compreendidos.
* Dependências identificadas e resolvidas.
* Estimativa de Story Points realizada.
* Equipe alinhada quanto ao objetivo da entrega.

### Definition of Done (DoD)

Uma funcionalidade só será considerada concluída se cumprir os seguintes critérios:

* Código revisado e integrado ao repositório.
* Testes automatizados implementados e passando.
* Deploy realizado em ambiente de homologação.
* Critérios de aceitação atendidos.
* **Requisitos Não Funcionais (RNF) atendidos:**
    * **Segurança (Login - RNF BSYNC-6):** Bloqueio da conta por 30 segundos após 5 falhas de login em 1 minuto.
    * **Performance (Cadastro - RNF BSYNC-5):** Retorno de sucesso do cadastro em menos de 2 segundos.
    * **Usabilidade/Acessibilidade (Dashboard - RNF BSYNC-7):** Botões de ação do dashboard (ex: alterar status) devem ser clicáveis e legíveis em dispositivo móvel.
    * **Performance (Busca - RNF BSYNC-9):** Exibição dos resultados da busca na Google Books API em no máximo 3 segundos.
    * **Confiabilidade/Limite (Avaliação - RNF BSYNC-8):** Sistema deve mostrar uma mensagem de erro e não criar uma avaliação duplicada caso o usuário já tenha avaliado o livro.
    * **Performance/Build Time (Infra - RNF BSYNC-29):** Imagem final do Docker deve ser construída em menos de 2 minutos.
    * **Otimização de Recursos (Infra - RNF BSYNC-32):** Apenas dependências essenciais devem ser instaladas no ambiente virtual.
    * **Segurança (Doc API - RNF BSYNC-31):** O campo de senha (`/login`) deve estar explicitamente marcado como *write-only* (não retornável na resposta).

---

## 📂 Artefatos de Entrega

Todos os artefatos do projeto estão disponíveis neste repositório.

| Artefato | Nome do Arquivo / Localização | Descrição |
| :--- | :--- | :--- |
| **Lean Inception & MVP Canvas (Miro)** | `lean-inception-Booksync.pdf` | Contém todas as etapas da Lean Inception e o MVP Canvas, conforme a atividade. |
| **Backlog do Produto (Jira)** | `backlog-bookSync.pdf` | Épicos (BSYNC-1 a BSYNC-4), Histórias de Usuário e Enablers, incluindo DoR e DoD. |
| **Backlog da Sprint 1 (Jira)** | `backlog-bookSync.pdf` | Detalhamento das Histórias de Usuário (ex: BSYNC-5, BSYNC-6, BSYNC-7, BSYNC-8, BSYNC-9) com Estimativas (Story Points: 5, 3, 5, 5, 2, respectivamente) e Critérios de Aceitação. |
| **Protótipos de Interface (Figma)** | `wireframes-booksync.pdf` | Protótipos de Baixa Fidelidade (wireframes) para Cadastro, Login, Busca, Avaliação e Dashboard (itens da Sprint 1). |
