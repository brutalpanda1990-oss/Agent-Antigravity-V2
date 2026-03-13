# 📖 Lessons Learned

> Erreurs passées et corrections. NE PAS répéter.

---

## Format

```
### [DATE] — [PROBLÈME]
**Symptôme** : [Ce qui s'est passé]
**Cause** : [Pourquoi]
**Solution** : [Comment corriger]
**Agent** : [Qui a détecté]
```

---

## Leçons initiales (V5)

### 2026-03-13 — Import de repos GitHub
**Symptôme** : L'IA bloque et génère une erreur quand on lui demande de lire un repo entier.
**Cause** : Context overflow. Charger des centaines de fichiers dépasse la fenêtre de contexte.
**Solution** : Toujours procéder fichier par fichier. Utiliser `/skill-import` avec le prompt anti-bloat. Jamais lire un repo complet en une seule passe.
**Agent** : skill-importer

### 2026-03-13 — Trop de skills simultanés
**Symptôme** : Activations parasites, réponses confuses, latence élevée.
**Cause** : Presets trop larges activés alors qu'un skill spécifique aurait suffi.
**Solution** : Règle anti-bloat : skill spécifique > preset général. Max 3 skills.
**Agent** : skill-router
