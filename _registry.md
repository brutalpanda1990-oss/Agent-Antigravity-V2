# 📚 Registre Central — V5.0

> **Agents** : 65 | **Skills** : 75 | **Alias** : 62 | **Presets** : 16 | **Commandes** : 20 | **Dernière màj** : 2026-03-13
> **Diff V4→4V5** : +7 agents, +14 skills, +7 alias, +1 preset, +2 commandes

---

## 🔗 Tous les Alias (62)

### Frontend (11)
| Alias | Skill | Chemin |
|---|---|---|
| `@react` | react-nextjs | skills/frontend/react-nextjs |
| `@react-bp` | react-best-practices | skills/frontend/react-best-practices |
| `@react-doctor` | react-doctor | skills/frontend/react-doctor |
| `@video` | remotion | skills/frontend/remotion |
| `@native` | native-ui | skills/frontend/native-ui |
| `@tw` | tailwind-css | skills/frontend/tailwind-css |
| `@state` | state-management | skills/frontend/state-management |
| `@a11y` | accessibility | skills/frontend/accessibility |
| `@seo` | seo-webvitals | skills/frontend/seo-webvitals |
| `@perf-profile` | performance-profiling | skills/frontend/performance-profiling |
| `@remotion` | remotion | skills/frontend/remotion |

### Design (5)
| Alias | Skill | Chemin |
|---|---|---|
| `@ui` | ui-ux | skills/design/ui-ux |
| `@canvas` | canvas | skills/design/canvas |
| `@theme` | theme-factory | skills/design/theme-factory |
| `@audit` | audit | skills/design/audit |
| `@radix` | radix-ui | skills/design/radix-ui |

### Backend (10)
| Alias | Skill | Chemin |
|---|---|---|
| `@db` | supabase-postgres | skills/backend/supabase-postgres |
| `@auth` | auth | skills/backend/auth |
| `@api` | api-design | skills/backend/api-design |
| `@cache` | caching-redis | skills/backend/caching-redis |
| `@supaauth` | nextjs-supabase-auth | skills/backend/nextjs-supabase-auth |
| `@prisma` | prisma | skills/backend/prisma |
| `@stripe` | stripe | skills/backend/stripe |
| `@inngest` | inngest | skills/backend/inngest |
| `@langsmith` | langsmith-fetch | skills/backend/langsmith-fetch |
| `@realtime` | realtime | skills/backend/realtime |

### IA & Data (4) — NOUVEAUX
| Alias | Skill | Chemin |
|---|---|---|
| `@ai-eng` | ai-engineer | skills/meta/ai-engineer |
| `@data` | data-analyst | skills/meta/data-analyst |
| `@rag` | rag | skills/meta/rag |
| `@llm` | llm-integration | skills/meta/llm-integration |

### Security (3)
| Alias | Skill | Chemin |
|---|---|---|
| `@security` | owasp-best-practices | skills/security/owasp-best-practices |
| `@sast` | sast-scanner | skills/security/sast-scanner |
| `@threats` | threat-modeling | skills/security/threat-modeling |

### Fullstack (5)
| Alias | Skill | Chemin |
|---|---|---|
| `@ts` | typescript-patterns | skills/fullstack/typescript-patterns |
| `@errors` | error-handling | skills/fullstack/error-handling |
| `@i18n` | i18n | skills/fullstack/i18n |
| `@clean` | clean-code | skills/fullstack/clean-code |
| `@debug-method` | debugging-strategies | skills/fullstack/debugging-strategies |

### DevOps (12)
| Alias | Skill | Chemin |
|---|---|---|
| `@git` | git-commit-helper | skills/devops/git-commit-helper |
| `@codereview` | code-reviewer | skills/devops/code-reviewer |
| `@mcp` | mcp-builder | skills/devops/mcp-builder |
| `@test` | webapp-testing | skills/devops/webapp-testing |
| `@docker` | docker-containers | skills/devops/docker-containers |
| `@cicd` | cicd-pipelines | skills/devops/cicd-pipelines |
| `@playwright` | playwright | skills/devops/playwright |
| `@sentry` | sentry | skills/devops/sentry |
| `@tdd` | tdd | skills/devops/tdd |
| `@changelog` | changelog-generator | skills/devops/changelog-generator |
| `@pr` | create-pull-request | skills/devops/create-pull-request |
| `@deploy` | vercel-deploy | skills/devops/vercel-deploy |

### Documents (3)
| Alias | Skill | Chemin |
|---|---|---|
| `@docx` | docx | skills/documents/docx |
| `@xlsx` | xlsx | skills/documents/xlsx |
| `@artifacts` | artifacts-builder | skills/documents/artifacts-builder |

### Personas (7) — +4 NOUVEAUX
| Alias | Skill | Chemin |
|---|---|---|
| `@sr-arch` | senior-architect | skills/personas/senior-architect |
| `@sr-back` | senior-backend | skills/personas/senior-backend |
| `@sr-front` | senior-frontend | skills/personas/senior-frontend |
| `@pm-expert` | product-manager | skills/personas/product-manager |
| `@content` | content-specialist | skills/personas/content-specialist |
| `@devops-arch` | devops-architect | skills/personas/devops-architect |
| `@ai-product` | ai-product-specialist | skills/personas/ai-product-specialist |

### Meta (7) — +1 NOUVEAU
| Alias | Skill | Chemin |
|---|---|---|
| `@meta` | skill-creator | skills/meta/skill-creator |
| `@prompts` | prompt-engineering | skills/meta/prompt-engineering |
| `@orchestrate` | agent-orchestration | skills/meta/agent-orchestration |
| `@skill-router` | skill-router | skills/meta/skill-router |
| `@skill-import` | skill-importer | skills/meta/skill-importer |
| `@verify` | verification | skills/meta/verification |
| `@skill-share` | skill-share | skills/meta/skill-share |

---

## ⚡ Presets (16) — +1 NOUVEAU

| Preset | Skills Inclus | Usage |
|---|---|---|
| `@fullstack` | react + db + auth + ui + ts + errors + security | Projet complet |
| `@frontend-complete` | react + ui + tw + state + a11y + seo + perf-profile | Frontend avancé |
| `@backend-complete` | db + auth + api + cache + security + prisma | Backend sécurisé |
| `@security-full` | security + sast + threats + auth + supaauth | Sécurité complète |
| `@security-audit` | security + sast + threats + api | Audit sécurité |
| `@testing-full` | test + playwright + tdd | Testing complet |
| `@quality-full` | clean + codereview + verify | Qualité code |
| `@performance` | react + seo + tw + cache + perf-profile | Optimisation perf |
| `@devops-full` | docker + cicd + sentry + git + changelog + pr + deploy | Pipeline complète |
| `@new-project` | react + db + auth + ui + ts + tw + errors + security + prisma | Démarrer un projet |
| `@design-full` | ui + canvas + theme + tw + a11y + radix | Design complet |
| `@ai-meta` | prompts + orchestrate + rag + ai-eng | IA & agents |
| `@debug` | errors + debug-method | Résoudre un problème |
| `@code-audit` | audit + react + db + security + codereview + clean | Review projet |
| `@documents` | docx + xlsx + artifacts | Documents |
| `@react-doctor-full` | react-doctor + perf-profile + state | **NOUVEAU** Diagnostic React |

---

## 📂 Skills Par Catégorie (75 total)

| Catégorie | Nb | Skills |
|---|---|---|
| frontend | 10 | react-nextjs, react-best-practices, react-doctor, remotion, native-ui, tailwind-css, state-management, accessibility, seo-webvitals, performance-profiling |
| design | 5 | ui-ux, canvas, theme-factory, audit, radix-ui |
| backend | 10 | supabase-postgres, auth, api-design, caching-redis, nextjs-supabase-auth, prisma, stripe, inngest, langsmith-fetch, realtime |
| security | 3 | owasp-best-practices, sast-scanner, threat-modeling |
| fullstack | 5 | typescript-patterns, error-handling, i18n, clean-code, debugging-strategies |
| devops | 12 | git-commit-helper, code-reviewer, mcp-builder, webapp-testing, docker-containers, cicd-pipelines, playwright, sentry, tdd, changelog-generator, create-pull-request, vercel-deploy |
| documents | 3 | docx, xlsx, artifacts-builder |
| personas | 7 | senior-architect, senior-backend, senior-frontend, product-manager, content-specialist, devops-architect, ai-product-specialist |
| meta | 9 | skill-creator, prompt-engineering, agent-orchestration, rag, verification, skill-share, skill-router, skill-importer, ai-engineer, data-analyst, llm-integration |

---

## 🔌 Commandes (20)

| Commande | Action |
|---|---|
| `/code-review` | Revue de code complète |
| `/create-prd` | Créer un PRD |
| `/refactor-code` | Refactoring guidé |
| `/ultra-think` | Réflexion approfondie |
| `/plan-sprint` | Planification sprint |
| `/debug-issue` | Debug systématique |
| `/security-scan` | Audit OWASP + SAST |
| `/deploy-checklist` | Checklist pré-deploy |
| `/performance-audit` | Audit performance |
| `/full-project-setup` | Setup projet complet |
| `/changelog` | Générer le changelog |
| `/create-pr` | Créer une Pull Request |
| `/netlify-deploy` | Déployer sur Netlify |
| `/clarify` | Clarifier une demande |
| `/clear` | Alias de /clarify |
| `/scan-skills` | Scanner les skills non enregistrés |
| `/bootstrap` | Scanner le projet et générer le contexte |
| `/status` | Afficher l'état des tâches |
| `/skill-import [url]` | **NOUVEAU** Importer un skill depuis un repo |
| `/react-doctor` | **NOUVEAU** Diagnostic React + performance |
