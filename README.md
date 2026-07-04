# MVP ChefAtHome - Gestão Ágil de Projetos e Produtos

Este repositório contém a documentação estratégica, o planejamento ágil e os artefatos de design de interface do MVP **ChefAtHome**, desenvolvido para a sprint de Gestão Ágil de Projetos e Produtos da PUC-Rio. O projeto consiste em um aplicativo/marketplace focado em conectar Chefs de Cozinha particulares a Anfitriões que desejam realizar eventos e experiências gastronômicas personalizadas em domicílio.

Para a concepção, gestão e materialização de todo o ecossistema do projeto, foram utilizadas de forma integrada três ferramentas essenciais de mercado: o **Miro** (para a facilitação do framework de concepção estratégica), o **Jira** (para o mapeamento e gerenciamento ágil do backlog) e o **Figma** (para o design de interface e prototipagem dos wireframes).

O objetivo principal desta entrega é validar o fluxo transacional crítico de contratação de forma simples, ágil e segura, utilizando esses frameworks para mitigar riscos de escopo e garantir valor desde o primeiro lançamento.

---

## 🧠 Concepção Estratégica (Miro)

A fase de *Discovery* do produto foi estruturada através da dinâmica de **Lean Inception** no Miro, alinhando os objetivos de negócio às necessidades reais dos usuários através das seguintes atividades:

- **Visão do Produto e "É / Não é - Faz / Não faz":** Delimitação clara das fronteiras de atuação do marketplace.
- **Personas e Jornadas do Usuário:** Mapeamento profundo dos dois lados da plataforma:
  - **Mariana (Anfitriã):** Busca praticidade, exclusividade e segurança ao contratar um chef para jantares em casa.
  - **Thiago (Chef):** Busca autonomia, visibilidade e uma plataforma simplificada para gerenciar sua agenda e menus.
- **Sequenciador de Ondas:** Divisão lógica dos incrementos do produto, garantindo a entrega do MVP funcional no menor tempo possível.
- **Parking Lot:** Utilizado estrategicamente para "estacionar" ideias de melhorias futuras mapeadas durante o processo (como edição de perfil e cabeçalhos com centrais de notificações globais), blindando o escopo da primeira sprint contra o risco de *scope creep*.

---

## 📊 Planejamento e Maturidade Ágil (Jira)

O escopo validado no Miro foi quebrado em um Product Backlog estruturado dentro do Jira, organizado por **Epics** de valor e estimado para execução.

- **Sprint 1 (Escopo do MVP):** Planejada com um total de **47 pontos de escolha**, focando estritamente no fluxo ponta a ponta de agendamento e resposta do prestador.
- **Estrutura dos Cards:** Cada User Story possui descrições ricas, critérios de aceitação rigorosos e regras claras de qualidade anexadas:
  - **Definition of Ready (DoR):** Critérios necessários para que uma tarefa possa entrar em desenvolvimento (história refinada, critérios de aceite claros, wireframe associado).
  - **Definition of Done (DoD):** Critérios para considerar a tarefa totalmente concluída (código revisado, testes executados, aderência ao design).

---

## 🎨 Prototipagem e UX/UI (Figma)

Para materializar o escopo planejado, os wireframes foram desenvolvidos adotando a abordagem *mobile-first*, com uma identidade visual limpa, consistente e minimalista. O fluxo contempla **8 telas integradas** que cobrem as seguintes jornadas:

### 🔐 Fluxo de Acesso e Segurança
- **01 - Login / Acesso:** Segmentação condicional imediata entre os papéis de Anfitrião e Chef através de elementos visuais claros.
- **02 - Cadastro de Anfitrião:** Formulário focado em conversão e captura de dados essenciais de cliente.
- **03 - Cadastro de Chef:** Captura de credenciais profissionais e links de portfólio externo.

### 🍽️ Fluxo do Prestador (Chef Thiago)
- **04 - Cadastro de Menu/Prato:** Cadastro simples do cardápio com inserção de ingredientes e modo de preparo, contando com um link de escape para o painel de pedidos caso o chef decida não cadastrar o menu no primeiro acesso.
- **08 - Painel de Pedidos (Home do Chef):** Central de gerenciamento estruturada em formato de *accordions* (sanfona), exibindo alertas de novos pedidos pendentes com dados de restrições alimentares da cliente e botões de ação direta para "Aceitar" ou "Recusar".

### 🧭 Fluxo da Cliente (Anfitriã Mariana)
- **05 - Vitrine de Cardápios (Home do Anfitrião):** Feed de rolagem contínua para busca e seleção visual de menus por tipo de culinária.
- **06 - Detalhes do Menu e Preço Dinâmico:** Tela de detalhes do prato que incorpora um contador numérico dinâmico de convidados, atualizando o valor total do serviço automaticamente em tempo real.
- **07 - Calendário e Solicitação de Agendamento:** Formulário estruturado de endereço, seleção de data/hora com microtexto de feedback de disponibilidade e resumo do valor total fixado em negrito acima do botão de confirmação.

---

## ♿ Acessibilidade

Visando a inclusão e a conformidade com as boas práticas de desenvolvimento de software, este projeto acompanha um documento descritivo de acessibilidade textual de todas as interfaces (`Descrição textual wireframes.docx`), garantindo que o fluxo, a disposição dos componentes e a hierarquia da informação possam ser interpretados com precisão por leitores de tela para usuários com deficiência visual.
