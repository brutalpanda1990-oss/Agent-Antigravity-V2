# 🔍 Auto-Discovery Protocol — V5.0

> Protocole pour détecter et intégrer automatiquement les nouveaux skills.

---

## Déclenchement

L'auto-discovery s'active quand :
1. Tu lances `/scan-skills`
2. Tu ajoutes un nouveau dossier dans `skills/` manuellement
3. Tu lances `/skill-import [url]`

---

## Protocole de détection

### Étape 1 : Scanner
Parcourir `skills/` et lister tous les dossiers qui contiennent un `SKILL.md`.

### Étape 2 : Valider le format
Chaque `SKILL.md` doit avoir :
```yaml
---
name: <nom-kebab-case>
description: "<Use when ...>"
---
```
Si le frontmatter est manquant ou invalide → alerter l'utilisateur.

### Étape 3 : Vérifier les collisions
Comparer avec `_registry.md` :
- Doublon de nom → proposer un rename
- Doublon de description → proposer une fusion
- Conflit de routing → alerter

### Étape 4 : Intégrer
1. Ajouter l'alias dans `_registry.md`
2. Ajouter le mot-clé dans `_routing-rules.md` si nécessaire
3. Confirmer à l'utilisateur

---

## Format officiel d'un skill

```
skills/<catégorie>/<nom-skill>/
├── SKILL.md           # Requis
├── scripts/           # Optionnel — scripts exécutables
├── examples/          # Optionnel — exemples d'usage
└── resources/         # Optionnel — références et templates
```

## Template SKILL.md

```markdown
---
name: <nom-kebab-case>
description: "Use when <cas d'usage précis en anglais>"
---

# Titre du Skill

## Use this skill when
- Cas 1
- Cas 2

## Do not use this skill when
- Exclusion 1 (pour éviter les activations parasites)

## Instructions
<Contenu du skill>

## Safety (si applicable)
⚠️ Limites et précautions
```

---

## Règles anti-bloat à respecter

1. Description TOUJOURS étroite — commencer par "Use when..."
2. Section "Do not use" OBLIGATOIRE
3. SKILL.md concis — longs exemples dans `examples/`, références dans `resources/`
4. Jamais activer un skill si son "Do not use" match la requête
5. Maximum 3 skills actifs par réponse
