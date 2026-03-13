# 📓 Decisions Journal

> Décisions techniques irréversibles. NE PAS contredire.

---

## Format

```
### [DATE] — [SUJET]
**Décision** : [Ce qui a été décidé]
**Raison** : [Pourquoi]
**Agent** : [Qui a décidé]
**Impact** : [Ce que ça change]
```

---

## Décisions initiales (V5)

### 2026-03-13 — Architecture système
**Décision** : Système global non lié à un projet. Adaptatif via `_project-context.md`.
**Raison** : Réutilisabilité maximale dans toutes les applications.
**Agent** : CTO
**Impact** : Les standards de code s'adaptent au projet actif, pas un stack fixé.

### 2026-03-13 — Anti-bloat
**Décision** : Maximum 3 skills actifs simultanément par réponse.
**Raison** : Éviter les crashes de contexte et les activations parasites.
**Agent** : CTO
**Impact** : Meilleure précision, moins de latence, moins d'erreurs.
