# CLAUDE.md — DTS Dépannage Elec

## Contexte du projet

Site web professionnel pour **DTS Dépannage Elec**, service
d'électricité urgence 24h/24 sur la zone frontalière franco-suisse.
Entreprise française (structure DTS — Déco Travaux Services).

---

## Stack technique

- **Framework** : Astro
- **CSS** : Tailwind CSS
- **Déploiement** : Vercel
- **Repo** : GitHub
- **Priorité absolue** : Mobile-first, PageSpeed > 90 sur mobile

---

## Identité visuelle

- **Nom** : DTS Dépannage Elec
- **Couleur principale** : Vert citron `#b8d400`
- **Couleur secondaire** : Bleu néon `#4ab3ff`
- **Fond** : Bleu marine sombre `#060d16`
- **Surface cards** : `#0a1e10`
- **Texte muted** : `#4a7a5a`
- **Style** : Sombre, néons verts/bleus, rappel électricité
- **Effets** : text-shadow néon sur les accents, glow sur les CTAs
- **Logo** : Carré DTS bleu marine avec texte vert citron

---

## Informations entreprise

- **Nom commercial** : DTS Dépannage Elec
- **Téléphone** : À compléter
- **Email** : À compléter
- **Adresse** : À compléter
- **Domaine** : À compléter (.fr)
- **Horaires** : 24h/24 — 7j/7
- **Tarifs journée** : 7h–19h
- **Tarifs nuit** : 19h–7h

---

## Tarifs (Prix HT)

### Journée — 7h à 19h
| Prestation | Prix HT |
|---|---|
| Déplacement | 75 € |
| Recherche de panne | 195 € |
| Main d'œuvre / heure | 90 € |
| Mise en sécurité électrique | 130 € |

### Nuit — 19h à 7h
| Prestation | Prix HT |
|---|---|
| Déplacement | 115 € |
| Recherche de panne | 230 € |
| Main d'œuvre / heure | 150 € |
| Mise en sécurité électrique | 145 € |

> Au-delà d'1h d'intervention, la main d'œuvre supplémentaire
> est facturée à l'heure. Devis signé avant tous travaux.
> Prix HT — TVA en vigueur applicable.

---

## Zones d'intervention

- Tout le Pays de Gex (01)
- Annemasse + 40 km (74)
- Thonon-les-Bains + 20 km (74)
- Annecy + 40 km (74)
- Bellegarde-sur-Valserine + 20 km (01)

### Villes principales à cibler en SEO
Gex, Ferney-Voltaire, Saint-Genis-Pouilly, Thoiry, Divonne,
Annemasse, Ville-la-Grand, Cranves-Sales, Saint-Julien-en-Genevois,
Thonon-les-Bains, Douvaine, Sciez, Annecy, Cran-Gevrier, Seynod,
Bellegarde, Châtillon-en-Michaille

---

## Services proposés

Focus **DÉPANNAGE UNIQUEMENT** — pas de travaux neufs.

1. Panne générale / coupure totale
2. Disjoncteur sauté (différentiel, sectionneur)
3. Tableau électrique (remplacement, mise aux normes)
4. Prises et éclairage
5. Mise en sécurité électrique
6. Urgence professionnelle (hôtels, restaurants, copropriétés)
7. Diagnostic / recherche de panne

---

## Architecture des pages

```
/ (accueil)
/depannage-electricite/          ← page pilier SEO 2000+ mots
/tarifs/
/zones/
/contact/

Pages villes SEO :
/electricien-urgence-gex/
/electricien-urgence-annemasse/
/electricien-urgence-ferney-voltaire/
/electricien-urgence-saint-julien/
/electricien-urgence-thonon/
/electricien-urgence-annecy/
/electricien-urgence-bellegarde/
/electricien-urgence-saint-genis-pouilly/
/electricien-urgence-divonne/
/electricien-urgence-thoiry/
/electricien-urgence-cranves-sales/
/electricien-urgence-ville-la-grand/
```

---

## Structure page d'accueil

1. **Barre urgence** (sticky)
   — Disponible 24h/24 — Intervention rapide — zones

2. **Navigation**
   — Logo + liens + bouton appel vert cliquable

3. **Hero**
   — Badge "Disponible maintenant" néon vert animé
   — H1 avec mots clés géo
   — Photo technicien en intervention (placeholder)
   — Bouton appel (gros, vert, tel:)
   — Bouton WhatsApp
   — 4 stats : Intervention rapide / 24h/7j / Tarif affiché / CB+Cash

4. **Nos interventions**
   — 6 services en grille 2 colonnes
   — Icônes SVG + prix de base

5. **Photos**
   — 3 photos : technicien / avant-après / matériel pro

6. **Nos engagements**
   — Tarif affiché
   — Devis avant travaux
   — Suivi J+1
   — Intervention rapide

7. **Zones d'intervention**
   — Grille 2 colonnes avec points néon verts

8. **Tarifs transparents**
   — 2 tableaux : journée et nuit

9. **Avis clients**
   — 3 avis avec étoiles et villes

10. **CTA final**
    — Fond vert — numéro + WhatsApp

11. **Bouton flottant mobile**
    — Toujours visible en bas de l'écran

12. **Footer**

---

## SEO — Règles importantes

### Balises meta sur CHAQUE page
```
title: [Mot clé + Ville] — DTS Dépannage Elec | Urgence 24h/24
description: Électricien urgence à [ville] ? DTS intervient
rapidement 24h/24 7j/7. Tarif affiché, devis avant travaux.
Appelez : [numéro]
```

### Schema.org LocalBusiness sur toutes les pages
```json
{
  "@type": "ElectricalContractor",
  "name": "DTS Dépannage Elec",
  "telephone": "À compléter",
  "openingHours": "Mo-Su 00:00-24:00",
  "areaServed": [
    "Pays de Gex",
    "Annemasse",
    "Thonon-les-Bains",
    "Annecy",
    "Bellegarde-sur-Valserine"
  ]
}
```

### H1 sur chaque page ville
```
Électricien urgence [Ville] — Intervention rapide 24h/24
```

### Maillage interne
— Chaque page ville pointe vers la page pilier
— La page pilier pointe vers toutes les pages villes
— Toutes les pages pointent vers /tarifs/ et /contact/

---

## Règles de conversion mobile OBLIGATOIRES

- Numéro téléphone cliquable `tel:` visible SANS scroller
- Bouton flottant permanent en bas sur mobile
- Bouton WhatsApp cliquable
- PAS de formulaire — uniquement appel direct
- Badge "Disponible maintenant" avec point vert animé
- PageSpeed > 90 mobile obligatoire

---

## Wording à utiliser

### À utiliser
- "Intervention rapide"
- "Disponible 24h/24 — 7j/7"
- "Tarif affiché"
- "Devis avant travaux"
- "Zéro surprise"
- "Appelez maintenant"
- "Réponse immédiate"

### À NE PAS utiliser
- "45 minutes" (ne pas promettre de délai précis)
- "Garantie 12 mois" (le technicien le dit sur place)
- "Pas cher" ou "moins cher"
- "Devis gratuit" (on ne fait pas de devis gratuit avant déplacement)

---

## Design — Règles importantes

- Fond sombre `#060d16` sur toutes les pages
- Effets néon vert sur les éléments clés (text-shadow)
- Effets néon bleu sur les titres de sections
- Point vert animé sur le badge "Disponible maintenant"
- Éclairs SVG discrets dans le fond du hero (rappel électricité)
- Cards avec border `rgba(184,212,0,0.1)` à `rgba(184,212,0,0.3)`
- Boutons CTA : `background #b8d400` + `box-shadow néon vert`
- Jamais de fond blanc — toujours sombre

---

## Photos à intégrer (à faire cette semaine)

- [ ] Technicien en tenue de travail (portrait professionnel)
- [ ] Technicien en intervention (tableau ouvert, câblage)
- [ ] Avant / après intervention
- [ ] Véhicule avec matériel pro
- [ ] Gros plan matériel électrique pro

---

## Notes importantes

- Entreprise française — pas d'intervention en Suisse officiellement
- Mettre en avant la proximité Genève comme argument de crédibilité
- Concurrents principaux : Léman Énergie, Chronoserv
- Différenciateur clé : SEUL à couvrir toute la zone avec tarif affiché
- TVA à préciser sur la page tarifs
- Paiement CB (terminal SumUp ou Stripe) + Cash sur place
