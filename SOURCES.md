# Sources consultees et verifiees (avril 2026)

Ce document recense les sources utilisees pour construire le skill `impots-fr`. A actualiser chaque annee apres publication de la loi de finances et mise a jour du BOFiP.

## Officielles (autorite)

### Codes et lois
- **Code General des Impots (CGI)** - Legifrance
  - Art. 194 a 197 : quotient familial, parts
  - Art. 156 : deductions du revenu global, deficit foncier
  - Art. 157 bis : abattement seniors
  - Art. 81 quater : heures supplementaires
  - Art. 81-36° : jobs etudiants < 26 ans
  - Art. 81 bis : apprentis
  - Art. 150 U : PV immobilieres
  - Art. 150 VH bis : PV actifs numeriques (seuil 305 €)
  - Art. 150 VB bis : reintegration amortissements LMNP (LF 2025)
  - Art. 155 B : regime impatries
  - Art. 163-0 A : systeme du quotient
  - Art. 163 quatervicies : PER, plafonds
  - Art. 199 sexdecies : emploi a domicile
  - Art. 199 octodecies : prestation compensatoire
  - Art. 199 novovicies : Denormandie
  - Art. 199 tervicies : Malraux
  - Art. 199 tricies : Loc'Avantages
  - Art. 199 terdecies-0 A : IR-PME/FIP/FCPI
  - Art. 199 unvicies : SOFICA
  - Art. 199 undecies B / C : Girardin industriel / logement social
  - Art. 199 decies H : investissement forestier
  - Art. 199 quater B : cotisations syndicales (credit)
  - Art. 199 quater F : frais de scolarite
  - Art. 200 : dons oeuvres
  - Art. 200-1 ter : dons Coluche
  - Art. 200-3 : dons partis politiques
  - Art. 200-0 A : plafonnement global niches 10 000 € / 18 000 €
  - Art. 200 A : PFU 30 % (31,4 % a partir de 2026)
  - Art. 200 quater B : garde enfant < 6 ans
  - Art. 200 quater C : borne de recharge (supprime au 01/01/2026)
  - Art. 200 sexdecies A : credit d'impot premier abonnement presse
  - Art. 154 bis : Madelin prevoyance/retraite TNS
  - Art. 224 : CDHR
  - Art. 979 : plafonnement IFI

- **Livre des Procedures Fiscales (LPF)**
  - Art. L64, L64 A : abus de droit
  - Art. L169 : delai de reprise (3 ans / 10 ans)

- **Loi de finances 2026** (adoptee fin 2025) :
  - Revalorisation bareme +0,9 %
  - Taux PAS individualise par defaut
  - CDHR reconduite
  - PER : report plafonds 3 -> 5 ans, fin deduction apres 70 ans
  - Deficit foncier double prolonge jusqu'au 31/12/2027
  - Dons Coluche : plafond 75 % porte a 2 000 € (dons >= 14/10/2025)
  - Jeanbrun : nouveau dispositif locatif
  - Relance logement : 3 ans, immeubles collectifs
  - Borne recharge : supprime 01/01/2026
  - CSG capital : 9,2 % -> 10,6 % (PFU 31,4 %)

- **Loi de finances 2025** et **loi Le Meur** (19/11/2024) :
  - Reforme LMNP : reintegration amortissements dans PV
  - Meubles tourisme non classes : seuil micro-BIC 15 000 €, abattement 30 %
  - Meubles tourisme classes : abattement 50 %

### BOFiP-Impots (bofip.impots.gouv.fr) - doctrine opposable
- BOI-IR-RICI-* : reductions et credits d'impot
- BOI-IR-RICI-30-* : frais de scolarite
- BOI-IR-RICI-390 : abonnement presse
- BOI-RSA-BASE-30-50 : frais professionnels reels
- BOI-RFPI-* : revenus fonciers
- BOI-RPPM-* : RCM, plus-values
- BOI-BIC-CHAMP-40 : LMNP/LMP
- BOI-BNC-* : BNC
- Actualite BOI 14449-PGP : deficit foncier double renovation energetique

### impots.gouv.fr
- Notices : 2041-NOT, 2041-GV (pensions), 2042, 2042-C, 2042-RICI, 2044, 2047, 2086, 3916, 3916-bis, 2042-IFI
- Simulateurs : bareme kilometrique, frais reels, impot sur le revenu
- Calendrier 2026 : declaration du 9 avril au 28 mai/4 juin 2026 selon departement
- FAQ borne electrique, emploi domicile, crypto

### Service-Public.gouv.fr
- F12 : emploi a domicile
- F9 : frais scolarite
- F14709 : PER
- F1419 : bareme IR
- F35578 : borne recharge
- F563 : IFI
- F2617 : heures supplementaires
- F32744 : location meublee
- F31130 : CEHR
- F31179 : plafonnement niches
- A14686 : bareme kilometrique 2026
- A18043 : forfait teletravail 2026
- A18045 : bareme IR 2026

### economie.gouv.fr / info.gouv.fr
- Loi de finances 2026 : synthese particuliers
- Campagne declaration 2026
- CDHR : mise en place et paiement

## Montants cles a verifier chaque annee

| Element | Valeur 2026 (revenus 2025) | Source |
|---------|---------------------------|--------|
| PASS 2025 | 47 100 € | Decret annuel |
| PASS 2026 | 48 060 € | Decret annuel |
| Plancher PER 2025 | 4 637 € | 10 % PASS 2024 |
| Plancher PER 2026 | 4 710 € | 10 % PASS 2025 |
| Plafond PER salarie max | 37 094 € (rev 2024) / ~35 194 € (rev 2025) | 10 % × 8 PASS N-1 |
| Bareme kilometrique | Inchange vs 2025 | Arrete annuel |
| Heures sup exoneration | 7 500 € (rev 2025) | Art. 81 quater |
| Emploi domicile plafond | 12 000 € / 15 000 € 1ere / 20 000 € handicap | Art. 199 sexdecies |
| Garde enfant < 6 ans | 3 500 €/enfant | Art. 200 quater B |
| Coluche plafond 75 % | 1 000 € puis 2 000 € (>= 14/10/2025) | LF 2026 |
| Plafond niches | 10 000 € / 18 000 € | Art. 200-0 A |
| CDHR seuils | 250 k€ / 500 k€, taux 20 % | Art. 224 |
| Crypto seuil cession | 305 € | Art. 150 VH bis |
| Assurance-vie abattement 8 ans | 4 600 € / 9 200 € | Art. 125-0 A |
| IFI seuil | 1,3 M€ | Art. 964 |
| Forfait mobilites durables | 600 € / 900 € | Art. 81-19° ter |
| Teletravail exoneration | 2,70 €/j ou 3,25 €/j (accord) | BOI-RSA-BASE |
| Frais scolarite | 61 / 153 / 183 € | Art. 199 quater F |
| Sanction 3916-bis | 750 € / 1 500 € / 125 € | Art. 1736 |

## Dispositifs supprimes ou modifies a suivre

- **Pinel** : fin 31/12/2024
- **CITE travaux energetiques** : supprime 01/01/2021 (remplace par MaPrimeRenov')
- **Censi-Bouvard** : fin 31/12/2022
- **Credit d'impot borne recharge** : fin 01/01/2026
- **FCPI classiques** : fin eligibilite 21/02/2026 (seuls FCPI JEI restent)
- **Credit d'impot abonnement presse** : modifie 14/02/2025, verifier prolongation

## Discipline de mise a jour

Ce skill doit etre revu :
- **Janvier** : nouvelle loi de finances, actualiser bareme, plafonds, nouveaux dispositifs
- **Mars-Avril** : ouverture campagne declaration, verifier cases formulaires
- **En cours d'annee** : lois de finances rectificatives, decrets d'application, bulletins BOFiP
