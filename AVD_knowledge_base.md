# Knowledge Base — Accelerated Value Delivery (AVD)
*Documento de contexto para iteração contínua do projeto*

---

## Sobre o Autor

**CP** — Engagement Manager na OutSystems (ou similar), com certificações em Product Management, Scrum Master e Project Manager. Não tem background técnico de desenvolvimento, mas nos últimos 3 semanas usou Claude + AI para construir e lançar 5–7 aplicações reais que resolvem problemas concretos — algo que nunca conseguiu fazer antes. Esta experiência prática é a base empírica do framework.

---

## O Problema que o Framework Resolve

O ciclo de entrega tradicional em plataformas como a OutSystems demora 3–4 meses (ou mais) do início ao primeiro valor entregue ao cliente. O ciclo típico é:

1. **Fase de Visão/Discovery** — 2 semanas
2. **Design, User Stories, Arquitetura** — 2 semanas
3. **Sprints de Desenvolvimento** — 6–8 sprints de 2 semanas
4. **QA e Release** — 2 semanas
5. **Suporte Pós-Produção** — contínuo

A métrica chave afectada é o **Time to First Value (TTV)** — o tempo desde o início até o cliente receber valor real. O argumento central do framework é que a IA torna este modelo obsoleto.

---

## O Framework: Accelerated Value Delivery (AVD)

### Premissa Central
A IA invalida as suposições que tornaram o Agile necessário. Um PM com ferramentas de IA consegue construir e entregar um MVP funcional em 2–3 dias, sem depender de silos de especialistas.

---

### FASE 1 — Rapid Discovery & MVP Build (Dias 1–3)

**Quem:** PM com ferramentas de IA + Product Owner + stakeholder de negócio directo + QA embebido

**Como funciona:**
- PM senta com o dono do negócio **directamente** — sem Business Analysts, sem intermediários
- Captura: problema central, objectivos, métricas de sucesso (a "visão")
- **Constrói imediatamente** com IA — sem user stories, sem wireframes entregues a designers
- **QA embebido em tempo real** — o especialista de qualidade trabalha ao lado do build, corrige on the fly
- **Sign-off diário do PO** — cada feature assinada formalmente à medida que é construída (audit trail claro)
- **Controlo de scope:** visão + objectivos + métricas mantidos visíveis; a IA alerta quando algo não contribui para os objectivos
- **Conflitos entre stakeholders:** IA gera matriz de impacto + pros/cons; PO toma a decisão final com transparência

**Output:** MVP funcional validado pelo PO ao fim do dia 3.

---

### FASE 2 — Technical Review & Hardening (Dias 4–5)

**Quem:** Arquitectos sénior + Tech Leads + Especialista UX de compliance

**Como funciona:**
- **Gate obrigatório** — nada vai a produção sem esta revisão (apps enterprise não são excepção)
- Scanning de segurança automatizado (não revisão manual linha a linha)
- Arquitectos focam em decisões de alto nível: integrações, infraestrutura, compliance
- IA gera documentação de compliance e relatórios de segurança automaticamente
- **Pattern library pré-aprovado** — validação contra componentes seguros conhecidos, não avaliação do zero
- UX: ADA, branding, acessibilidade — track paralelo, não bloqueador
- O objectivo é **compressão máxima** com ferramentas de IA, não cortar corners

**Output:** Aplicação pronta para produção. **Deployment no início da semana seguinte.**

---

### FASE 3 — Continuous Evolution via Stakeholder Sandboxing (Contínuo)

**Quem:** Stakeholders relevantes (certificados) + Product Owner + Agentes automatizados

**Como funciona:**

**Modelo de Sandbox:**
- Qualquer stakeholder **treinado e certificado** pode criar um sandbox pessoal — cópia isolada da app em produção
- Constrói novas features com IA dentro do sandbox
- Sandbox é **completamente isolado** da produção — nenhum risco ao sistema live

**Processo de Votação:**
- Submete a feature ao grupo de **stakeholders relevantes** (não à empresa toda — apenas quem tem skin in the game)
- Votos = sinal de prioridade, não mandato
- **PO toma a decisão final** e explica publicamente as rejeições (transparência obrigatória)

**Ideias rejeitadas:**
- Não são eliminadas — são **arquivadas com contexto** (razão da rejeição)
- O proponente decide o destino do próprio sandbox (continuar a iterar ou arquivar)
- Auto-archive por inactividade (política a definir) para controlo de custos

**Responsabilidades dos Agentes Automatizados:**
1. **Detecção de duplicados** — escaneia sandboxes activos, sugere merges de ideias similares
2. **Monitor de estratégia** — quando os objectivos mudam, ressurface ideias anteriormente rejeitadas que agora fazem sentido
3. **Gestão de arquivo** — auto-arquiva sandboxes inactivos

---

## Modelo de Governança

| Papel | Modelo Antigo | Modelo AVD |
|-------|--------------|------------|
| Product Owner | Gestor de backlog / escritor de stories | Autoridade de decisão + revisor diário + dono do sign-off |
| Business Analyst | Intermediário de requisitos | Eliminado — substituído por conversa directa stakeholder-PM |
| Arquitecto / Tech Lead | Revisão de várias semanas | Gate técnico de 1–2 dias com IA e scanning automatizado |
| QA Tester | Testes pós-desenvolvimento | Qualidade em tempo real embebida no build |
| UX Designer | Wireframes upfront | Revisão pós-MVP: ADA, branding, acessibilidade |
| PM / Engagement Manager | Coordenador / facilitador | Builder principal — com superpoderes de IA |

**Hierarquia de decisão:**
- PO tem autoridade final sobre o que vai a produção
- Conflitos entre stakeholders → IA gera análise de impacto; PO decide
- Hierarquia (ex: CEO) pode sobrepor-se, mas deve articular o raciocínio — o processo torna as decisões visíveis

---

## Modelo de Segurança (Sandbox)

1. **Isolamento total** — sandboxes sem acesso a dados ou infraestrutura de produção
2. **Scanning automatizado** — todo o código escaneado antes de chegar à revisão da comunidade
3. **Permissões por role** — áreas sensíveis (auth, pagamentos, exports) bloqueadas a roles privilegiados
4. **Code review gate** — arquitectos sénior revêem antes de qualquer feature chegar a produção
5. **Audit trails** — rastreabilidade completa de quem mudou o quê, quando e porquê

---

## Treino e Certificação

- Participação no sandbox é **opt-in por auto-selecção** (motivação natural)
- Treino obrigatório antes de acesso ao sandbox (modelo: certificações Power BI, Snowflake, etc.)
- Profissionais experientes também assinam confirmação de que compreendem o novo modo de trabalho
- Resultado: só pessoas motivadas e formadas participam — qualidade por design

---

## Gaps Identificados e Resolvidos

| Gap | Solução |
|-----|----------|
| Scope creep | Visão + objectivos + métricas visíveis; IA alerta quando features não contribuem para os goals |
| Accountability de requisitos | PO embebido, revê diariamente, sign-off formal por feature |
| Conflitos entre stakeholders | IA gera análise de impacto; PO decide com transparência |
| Votação vs. estratégia de negócio | Votos são sinal de prioridade, não mandato; PO tem palavra final |
| Rejeições e frustração | PO explica rejeições publicamente; ideias rejeitadas são arquivadas, não eliminadas |
| Sandboxes obsoletos | Proponente decide; auto-archive por inactividade |
| Segurança no modelo descentralizado | 5 camadas: isolamento, scanning, roles, code review, audit trail |
| Treino de não-developers | Certificação obrigatória antes de acesso ao sandbox |
| Velocidade da revisão técnica | AI tools + scanning automatizado + pattern library = compressão máxima |

---

## Métricas Alvo

| Métrica | Antes | AVD |
|---------|-------|-----|
| Time to First Value | 3–4 meses | 1 semana |
| Taxa de escape de defeitos | Pós-sprint | Próxima de zero |
| Cadência de sign-off do PO | Fim de sprint | Diária |
| Feature nova a produção | 2–4 semanas | Dias |
| Participação de stakeholders | Mediada pelo PO | Directa |

---

## Deliverables Já Produzidos

1. **Paper** — `ai_delivery_framework_paper.md` — documento completo com abstract, 8 secções, conclusão
2. **Visual Workflow** — `avd_workflow.html` — diagrama interactivo dark theme com todas as fases
3. **Slide Deck** — `avd_presentation.pptx` — 11 slides, design dark executive (Cambria + Calibri)

---

## Próximos Passos Sugeridos para Iteração

- [ ] Definir o nome final do framework (confirmar "Accelerated Value Delivery" ou alternativa)
- [ ] Adicionar o nome do autor no paper e nos slides
- [ ] Expandir a secção de casos reais — as 5–7 apps construídas por CP são evidência empírica poderosa
- [ ] Explorar comparação formal com frameworks existentes (SAFe, Shape Up, BMAD Method)
- [ ] Definir métricas de adopção: como se mede o sucesso do próprio framework?
- [ ] Considerar um piloto real — proposta de como testar o AVD num projecto OutSystems

---

*KB v1.0 — Gerado a partir de conversa completa de ideação com CP*
