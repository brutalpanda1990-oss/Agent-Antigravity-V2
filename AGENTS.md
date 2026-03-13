# AGENTS.md — Gouvernance Universelle

> Ce fichier gouverne le comportement de TOUS les coding agents (Antigravity, Claude, Copilot, Cursor) sur ce repo.
> Version : 2.0 | Dernière màj : 2026-03-13

---

## 🌐 Portée

Ce fichier s'applique à **toute interaction agent** sur ce repository, quel que soit l'outil utilisé.

---

## 📋 Conventions obligatoires

### Langue
- Code : **anglais** (noms de variables, fonctions, commentaires)
- Réponses à l'utilisateur : **français**
- Messages de commit : **anglais** (Conventional Commits)

### Commits
Format strict : `type(scope): description`
- `feat(auth): add JWT refresh endpoint`
- `fix(ui): correct button alignment on mobile`
- `docs(readme): update installation guide`

Types autorisés : `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `perf`, `ci`

### Fichiers et dossiers
- Composants React : `PascalCase.tsx`
- Utils et services : `camelCase.ts`
- Dossiers : `kebab-case/`
- Constantes globales : `UPPER_SNAKE_CASE`

---

## 🚫 Limites des agents

### Ce que les agents NE FONT PAS
- Ne jamais créer de compte, payer, envoyer d'email sans confirmation explicite
- Ne jamais supprimer de base de données en production
- Ne jamais hardcoder de secrets, clés API ou tokens
- Ne jamais bypasser les tests ou les gates de qualité
- Ne jamais sortir du scope de la tâche demandée

### Escalade obligatoire
L'agent doit demander confirmation avant :
- Suppression de fichiers ou données critiques
- Changement d'architecture majeur
- Migration de base de données
- Modification de fichiers `.env` ou de config de production

---

## 🧭 Routing des agents

Le routing est géré par `_routing-rules.md`. En résumé :
1. Le **Dispatcher** (Level 0) analyse chaque prompt
2. Il route vers l'agent Level 1-4 le plus pertinent
3. Les skills sont chargés **à la demande** (progressive disclosure)
4. Maximum **3 skills actifs simultanément** par tour

---

## 📁 Structure du projet

Voir `README.md` pour l'arborescence complète.

---

## ✅ Checklist de qualité (obligatoire)

Tout code livré doit passer :
- [ ] TypeScript strict (pas de `any`)
- [ ] Error handling complet (try/catch sur tout async)
- [ ] Validation inputs (Zod ou équivalent)
- [ ] 0 secret hardcodé
- [ ] Tests unitaires pour la logique métier
- [ ] Review automatique de l'agent code-reviewer

---

## 🔧 Intégration de skills externes

Pour importer un skill depuis un repo externe :
1. Utiliser la commande `/skill-import [url-repo]`
2. L'agent `meta/skill-importer` class l'élément (skill / persona / resource / règle)
3. Conversion au format `SKILL.md` Antigravity officiel
4. Test du routing après chaque ajout
5. Maximum 5 skills ajoutés par session

---

> Ce fichier est la référence universelle. En cas de conflit avec d'autres fichiers, `AGENTS.md` a priorité sauf pour `SYSTEM.md` sur les standards de code.
