# 🦭 Routing Rules — V3.0

> Règles d'auto-routing pour le Dispatcher.
> L'utilisateur ne nomme JAMAIS un agent. Le système route automatiquement.
> V3 : +react-doctor, +ai-engineer, +data-analyst, +product-manager, +skill-importer, +anti-collision

---

## Règle 0 : Anti-Bloat (PRIORITÉ CRITIQUE)

Avant tout routing :
1. **Maximum 3 skills actifs** par réponse — choisir les plus spécifiques
2. **Skill spécifique > preset général** — ne jamais activer @fullstack si @react suffit
3. Si la demande touche 4+ domaines → activer `meta/skill-router` en premier
4. En cas de collision de routing → choisir l'agent de niveau le plus bas (le plus spécialisé)

---

## Règle 1 : Contexte de Fichier (PRIORITÉ HAUTE)

| Extension / Path | Agent par défaut | Skills auto-chargés |
|---|---|---|
| `.tsx` / `.jsx` | react-developer | @react |
| `.css` / `.scss` | css-tailwind-expert | @tw |
| `.ts` (non-React) | typescript-expert | @ts |
| `route.ts` / `api/` | api-designer | @api, @security |
| `.sql` / `migrations/` | database-engineer | @db, @prisma |
| `Dockerfile` | docker-specialist | @docker |
| `.test.ts` | testing-lead | @test |
| `.md` / `.mdx` | documentation-lead | — |
| `package.json` | devops-lead | @ts |
| `.env` | security-lead | @security |
| `tailwind.config.ts` | css-tailwind-expert | @tw |
| `auth.ts` | auth-specialist | @auth, @security |
| `*.ipynb` | data-analyst | @data |
| `langchain/` / `rag/` | ai-llm-engineer | @rag, @langsmith |

---

## Règle 2 : Verbes d'Action (PRIORITÉ MOYENNE)

| Verbe français | Agent par défaut |
|---|---|
| Créer / Construire / Ajouter | Lead du domaine |
| Corriger / Fixer / Débugger | bug-hunter |
| Diagnostiquer React / profiler | react-doctor |
| Optimiser / Accélérer | performance-lead |
| Sécuriser / Protéger | security-lead |
| Tester / Vérifier | testing-lead |
| Documenter / Expliquer | documentation-lead |
| Déployer / Mettre en prod | devops-lead |
| Planifier / Organiser | project-manager |
| Restructurer / Refactorer | cto |
| Designer / Maquetter | design-lead |
| Auditer / Reviewer | qa-director |
| Analyser les données / Dashboard | data-analyst |
| Intégrer un LLM / RAG | ai-engineer |
| Importer un skill / repo | skill-importer |
| Définir produit / user story | product-manager |
| Migrer / Upgrader | cto + devops-lead |

---

## Règle 3 : Mots-clés Spécifiques (PRIORITÉ BASSE)

### Frontend
| Mots-clés | Agent | Skills |
|---|---|---|
| composant, hook, useState, useEffect | react-developer | @react |
| react lent, re-render, profiler, memo | react-doctor | @react-doctor |
| page, layout, route, App Router | nextjs-specialist | @react |
| CSS, Tailwind, style, responsive | css-tailwind-expert | @tw |
| state, zustand, context, React Query | state-management-expert | @state |
| animation, motion, framer, GSAP | animation-specialist | @react |
| a11y, ARIA, screen reader | accessibility-expert | @a11y |
| SEO, meta, Open Graph, sitemap | seo-specialist | @seo |

### Backend
| Mots-clés | Agent | Skills |
|---|---|---|
| API, endpoint, REST, GraphQL | api-designer | @api |
| base de données, SQL, migration | database-engineer | @db |
| auth, login, JWT, OAuth | auth-specialist | @auth, @security |
| realtime, WebSocket, live | realtime-engineer | @db |
| cache, Redis, CDN | cache-specialist | @cache |

### IA & Data (NOUVEAU)
| Mots-clés | Agent | Skills |
|---|---|---|
| LLM, modèle IA, embedding, RAG | ai-engineer | @ai-eng, @rag |
| LangSmith, LangChain, trace AI | ai-llm-engineer | @langsmith |
| data, dashboard, métriques, rapport | data-analyst | @data |
| prompt engineering, fine-tune | ai-engineer | @prompts |

### Fullstack
| Mots-clés | Agent | Skills |
|---|---|---|
| TypeScript, type, generic | typescript-expert | @ts |
| erreur, error, logging, Sentry | error-handling-specialist | @errors |
| i18n, multilingue, traduction | i18n-specialist | @i18n |

### DevOps
| Mots-clés | Agent | Skills |
|---|---|---|
| Docker, container, compose | docker-specialist | @docker |
| CI/CD, GitHub Actions | cicd-engineer | @cicd |
| déployer, Vercel, staging | deployment-specialist | @deploy |
| monitoring, logs, alertes | monitoring-engineer | @sentry |
| service gratuit, free tier | devops-lead | @free-tools |

### Design
| Mots-clés | Agent | Skills |
|---|---|---|
| design, UI, bouton, modal | ui-designer | @ui |
| UX, parcours, wireframe | ux-researcher | @ui |
| design system, tokens, thème | design-system-architect | @theme |

### Personas & Meta
| Mots-clés | Agent | Skills |
|---|---|---|
| produit, feature, user story, backlog | product-manager | @pm-expert |
| contenu, copywriting, rédaction | content-specialist | @content |
| skill, importer, repo externe, intégrer | skill-importer | @skill-import |
| infrastructure, cloud, IaC | devops-architect | @devops-arch |

---

## Règle 4 : Escalade Automatique

| Situation | Action |
|---|---|
| Agent Level 3 bloqué | → Escalade au Lead (Level 2) |
| Lead bloqué | → Escalade au CTO (Level 1) |
| Choix de priorité | → Escalade au PM |
| Problème de qualité | → Escalade QA Director |
| Conflit entre agents | → CTO pour arbitrage |
| Prompt ambigu | → Prompt Clarifier |
| Domaine 4+ simultanément | → skill-router |

---

## Règle 5 : Post-Exécution Automatique

| Ordre | Agent | Condition |
|---|---|---|
| 1 | code-reviewer-senior | TOUJOURS |
| 2 | bug-hunter | TOUJOURS (sauf CSS-only) |
| 3 | security-auditor | Si API, auth, database |
| 4 | accessibility-expert | Si UI, composant, page |
| 5 | performance-profiler | Si changement critique |
| 6 | unit-test-writer | Si logique métier |

---

## Règle 6 : Prompt Clarifier

| Condition | Action |
|---|---|
| Prompt > 200 mots | Clarifier résume et structure |
| Prompt vague | Clarifier pose des questions |
| Multi-tâches non structuré | Clarifier décompose |
| Contradictions | Clarifier les identifie |
| Demande d'import de repo complet | Clarifier + procéder fichier par fichier |
