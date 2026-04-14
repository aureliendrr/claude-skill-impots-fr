# impots-fr — Skill Claude pour optimiser sa declaration d'impots (France)

Un skill [Claude Code](https://docs.claude.com/claude-code) / Claude.ai qui transforme Claude en conseiller fiscal pour particuliers francais. L'objectif : poser **toutes** les bonnes questions pour identifier chaque euro d'economie d'impot **legale et sourcee** a la declaration 2026 (revenus 2025).

> Pas de conseil financier, pas de montage douteux, pas d'hallucination fiscale. Chaque recommandation cite son article CGI, BOFiP ou notice impots.gouv.fr.

## A quoi ca sert

Tu declenches le skill (ou il se declenche tout seul quand tu parles d'impots), et Claude deroule un questionnaire exhaustif en **6 vagues** pour ne rien oublier :

1. **Foyer fiscal** — situation, enfants, handicap, ages, residence
2. **Revenus** — salaires, pensions, fonciers, RCM, PV mobilieres, crypto, meubles tourisme
3. **Arbitrages structurants** — frais reels vs 10 %, PFU vs bareme, micro vs reel, rattachement vs pension, LMNP
4. **Reductions / credits d'impot** — emploi domicile, garde enfant, dons, PER, FIP/FCPI, SOFICA, Girardin, Loc'Avantages, Denormandie, Jeanbrun, etc.
5. **Situations specifiques** — impatries, frontaliers, < 26 ans, handicap, IFI
6. **Verifications finales** — plafonnement niches 10 k€, CDHR, justificatifs

A la fin : synthese chiffree avec cases de declaration (7UF, 7DB, 6QS, 4BE...), arbitrages recommandes, documents a reunir, sources.

## Installation

### Claude Code (CLI)

```bash
git clone https://github.com/aureliendrr/claude-skill-impots-fr.git
ln -s "$(pwd)/claude-skill-impots-fr" ~/.claude/skills/impots-fr
```

Puis dans une conversation : `/impots` ou parle juste de "declaration d'impots", "PER", "credit d'impot", etc. — le skill se declenche.

### Claude.ai (web/desktop)

Copie le contenu de `SKILL.md` dans un Project ou dans une instruction systeme personnalisee.

## Contenu du repo

| Fichier | Role |
|---------|------|
| `SKILL.md` | Prompt complet du skill, declencheurs, methode, sources |
| `SOURCES.md` | Table des articles CGI / BOI / notices utilises, montants cles 2026, discipline de MAJ |
| `README.md` | Ce fichier |

## Ce qui est couvert (non exhaustif)

- Bareme IR 2026 revalorise (+0,9 %), taux PAS individualise par defaut
- **CDHR** (taux minimum 20 % sur hauts revenus > 250/500 k€)
- **PFU** 30 % (revenus 2025) → 31,4 % a partir de 2026
- **PER** : plafonds 2026, report 5 ans, fin deduction apres 70 ans
- **Pinel** supprime 31/12/2024 → **Jeanbrun** et **Relance logement** (LF 2026)
- **LMNP** : reforme loi Le Meur, reintegration amortissements dans PV
- **Meubles tourisme** : nouveaux seuils/abattements (15 k€ / 30 % non classe)
- **Deficit foncier** double 21 400 € prolonge jusqu'au 31/12/2027
- **Dons Coluche** : plafond 75 % porte a 2 000 € (dons ≥ 14/10/2025)
- **Emploi a domicile** (12/15/18/20 k€ selon cas)
- **FIP/FCPI/IR-PME** : taux 18/25/30 % selon cible (JEI, Corse, DROM)
- **Girardin** industriel et logement social OM
- **SOFICA**, Malraux, Monuments historiques, Denormandie, Loc'Avantages
- **Crypto** : PFU, seuil 305 €, 3916-bis obligatoire
- **Frais reels**, bareme kilometrique, teletravail, forfait mobilites durables
- **IFI** 1,3 M€, abattement 30 % RP, plafonnement 75 %
- Frais scolarite, garde d'enfant, pension alimentaire, prestation compensatoire
- Impatries, frontaliers, < 26 ans, apprentis, stagiaires

## Ce qui n'est PAS couvert

- Fiscalite des entreprises (IS, TVA, CFE/CVAE)
- Succession / donation (hors signalement)
- Contentieux, reclamation, controle fiscal
- Fiscalite internationale complexe (holdings, trusts, expatriation)

Pour ces cas : **expert-comptable ou avocat fiscaliste obligatoire**.

## Avertissement

Ce skill est un **assistant de preparation**, pas un conseil fiscal engageant. Les regles evoluent (loi de finances annuelle, decrets, BOFiP). L'auteur decline toute responsabilite. Verifie toujours sur [impots.gouv.fr](https://www.impots.gouv.fr) et consulte un professionnel pour les situations complexes (LMNP, IFI, CDHR, impatries, PV immobilieres avec demembrement).

## Sources principales

- [impots.gouv.fr](https://www.impots.gouv.fr) — notices officielles, simulateurs
- [bofip.impots.gouv.fr](https://bofip.impots.gouv.fr) — doctrine administrative opposable
- [Legifrance](https://www.legifrance.gouv.fr) — CGI et LPF a jour
- [service-public.gouv.fr](https://www.service-public.gouv.fr) — vulgarisation officielle
- Loi de finances 2026 (adoptee fin 2025)

## Mise a jour

A reviser chaque annee apres publication de la loi de finances (decembre/janvier). Voir `SOURCES.md` pour la checklist des points a verifier.

## Licence

MIT — utilise, modifie, partage librement.

## Contribuer

Issues et PRs bienvenues. En particulier : nouveaux dispositifs LF, corrections de plafonds, ajouts de cas limites, cases de declaration.
