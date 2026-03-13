# 🗻️ Agent Hierarchy Map — V5.0

> 65 agents, 5 niveaux hiérarchiques. Système global et réutilisable.

---

## 🏗️ Structure des 5 Niveaux

### Level 0 — Dispatch (2 agents)
| Agent | Rôle |
|---|---|
| `dispatcher` | Point d'entrée unique. Analyse, clarifie et route. |
| `prompt-clarifier` | Structure les demandes vagues avec choix A/B/C. |

### Level 1 — Directors (3 agents)
| Agent | Rôle |
|---|---|
| `cto` | Gardien de l'architecture et de la vision technique. |
| `project-manager` | Sprint planning, roadmap, suivi de progression. |
| `qa-director` | Qualité globale, validation finale, gates de qualité. |

### Level 2 — Leads (8 agents)
| Agent | Domaine |
|---|---|
| `frontend-lead` | React 19, Vite, Tailwind |
| `backend-lead` | Supabase, API Design, Sécurité |
| `design-lead` | Design System, UI/UX |
| `devops-lead` | Déploiement, CI/CD, Changelog |
| `security-lead` | Audit OWASP, Threat Modeling |
| `testing-lead` | Tests, Coverage, TDD |
| `performance-lead` | Core Web Vitals, Bundle Size |
| `documentation-lead` | README, JSDoc, Guides |

### Level 3 — Developers (35 agents)

#### Frontend (8)
| Agent | Spécialité |
|---|---|
| `react-developer` | Composants, Hooks, State |
| `react-doctor` | **NOUVEAU** Diagnostic performance React, re-renders |
| `nextjs-specialist` | App Router, Server Components |
| `css-tailwind-expert` | Styling, Responsive, Animations |
| `state-management-expert` | Zustand, React Query, Context |
| `animation-specialist` | Framer Motion, GSAP |
| `accessibility-expert` | ARIA, a11y, Screen readers |
| `seo-specialist` | Meta, Open Graph, Sitemap |

#### Backend (7)
| Agent | Spécialité |
|---|---|
| `api-designer` | REST, GraphQL, OpenAPI |
| `database-engineer` | SQL, Migrations, Indexing |
| `auth-specialist` | JWT, OAuth, RLS, MFA |
| `realtime-engineer` | WebSocket, Supabase Realtime |
| `cache-specialist` | Redis, CDN, Edge |
| `integration-engineer` | Stripe, Webhooks, MCP, APIs externes |
| `ai-llm-engineer` | Gemini, LangChain, RAG, Embeddings |

#### IA & Data (3) — NOUVEAUX
| Agent | Spécialité |
|---|---|
| `ai-engineer` | Intégration LLM, Prompt Engineering, Fine-tuning |
| `data-analyst` | Dashboard, Métriques, Rapports, Visualisation |
| `rag-specialist` | Retrieval-Augmented Generation, Vector DB |

#### Fullstack (5)
| Agent | Spécialité |
|---|---|
| `typescript-expert` | Types, Generics, Utility Types |
| `error-handling-specialist` | Error Boundaries, Logging, Monitoring |
| `i18n-specialist` | Multilingue, RTL, Localisation |
| `performance-profiler` | React Profiler, Bundle Analyzer |
| `debugging-specialist` | Debug systématique, Root Cause Analysis |

#### DevOps & Infrastructure (6)
| Agent | Spécialité |
|---|---|
| `docker-specialist` | Containers, Images, Compose |
| `cicd-engineer` | GitHub Actions, Pipelines |
| `deployment-specialist` | Vercel, Netlify, Staging |
| `monitoring-engineer` | Sentry, Logs, Alertes |
| `mcp-builder` | Model Context Protocol |
| `git-specialist` | Commits, Branches, Merge Strategy |

#### Design (3)
| Agent | Spécialité |
|---|---|
| `ui-designer` | Composants UI, Radix, Shadcn |
| `ux-researcher` | User Flows, Wireframes, Personas |
| `design-system-architect` | Tokens, Thèmes, Design Language |

### Level 4 — Quality (13 agents)
| Agent | Rôle |
|---|---|
| `code-reviewer-senior` | Review systématique, score /100 |
| `bug-hunter` | Diagnostic SYSTEMATIC, Root Cause Analysis |
| `security-auditor` | OWASP, SAST, CVE, Vulnérabilités |
| `unit-test-writer` | Jest, Vitest, Tests unitaires |
| `integration-test-writer` | Tests d'intégration, API tests |
| `e2e-test-writer` | Playwright, Cypress |
| `tdd-coach` | TDD, Red-Green-Refactor |
| `performance-auditor` | Core Web Vitals, Lighthouse |
| `accessibility-auditor` | WCAG, Keyboard Nav |
| `documentation-reviewer` | Qualité de la documentation |
| `type-checker` | TypeScript strict, type safety |
| `dependency-auditor` | npm audit, CVE, Licences |
| `skill-importer` | **NOUVEAU** Import/conversion skills externes |

---

## 📚 Personas Spécialisées (7) — NOUVEAUX

| Persona | Rôle |
|---|---|
| `senior-architect` | Vision technique haut niveau |
| `senior-backend` | Backend senior patterns |
| `senior-frontend` | Frontend senior patterns |
| `product-manager` | Product specs, user stories, OKRs |
| `content-specialist` | Copywriting, rédaction technique |
| `devops-architect` | Infrastructure as Code, Cloud |
| `ai-product-specialist` | Produits IA, intégration LLM |

---

## ⚡ Interaction des Agents

1. **Dispatch** : Dispatcher analyse et route
2. **Planning** : PM + CTO définissent le blueprint
3. **Execution** : Leads et Developers implémentent
4. **Quality** : Level 4 valide systématiquement
5. **Escalade** : Niveau inférieur bloqué → escalade automatique au niveau supérieur
