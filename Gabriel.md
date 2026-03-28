# horaire-serie-2026
# 🏒 Tournoi Séries 2026 - Chemins de Dépendances
## 🟣 HUSKY 1 (m21c) - Gabriel

### Structure des Dépendances

```mermaid
graph TD
    M21C07["Lost MATCH 7<br/>HUSKY 1 (2) @ SEIGNEURS 2 (4)<br/>(28 mars 16:00)<br/>Lévis"] 
    M21C10["🔴 MATCH 10<br/>Perdant #7<br/>(29 mars 19:00)<br/>Saint-Nicolas"]
    M21C10 -->|Gagnant| M21C12["MATCH 12<br/>Gagnant #10<br/>(4 avril 18:00)<br/>Saint-Agapit"]
    M21C12 -->|Gagnant| M21C15["MATCH 15<br/>Gagnant #12<br/>(5 avril 16:00)<br/>Sainte-Marie"]
    M21C15 -->|Gagnant| M21C18["MATCH 18<br/>Gagnant #15<br/>(11 avril 16:00)<br/>Lévis"]
    M21C18 -->|Gagnant| M21C19["MATCH 19<br/>Gagnant #18<br/>(11 avril 20:30)<br/>Lévis"]
    M21C19 -->|Gagnant| M21C20["🟡 MATCH 20<br/>FINALE<br/>(12 avril 11:30)<br/>Saint-Agapit"]
    M21C10 -->|Perdant| K["Fin de la saison"]
    M21C12 -->|Perdant| K["Fin de la saison"]
    M21C15 -->|Perdant| K["Fin de la saison"]
    M21C16 -->|Perdant| K["Fin de la saison"]
    M21C19 -->|Perdant| K["Fin de la saison"]
    M21C18 -->|Gagnant| L["Régionnaux"]

    linkStyle 0,1,2,3,4,10 stroke:#22c55e,stroke-width:2.5px
    linkStyle 5,6,7,8,9 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    

```

### 📍 Chemins Vers la FINALE (Match 20)

| Match | Chemins Possibles | Nombre de Chemins |
|-------|-------------------|-------------------|
| **7** | DIRECT | 1 |
| **10** | L7 | 1 |
| **12** | L7 → W10 | 1 |
| **15** | L7 → W10 → W12 | 1 |
| **18** | L7 → W10 → W12 → W15 | 1 |
| **19** | L7 → W10 → W12 → W15 → W18 | 1 |
| **20** | L7 → W10 → W12 → W15 → W18 → W19 | 1 |

---

## 📈 Statistiques


## 🔑 Légende

- **W#** = Gagnant du match #
- **L#** = Perdant du match #
- **OU** = Chemin alternatif possible
- 🔴 = Match initial (garantis)
- 🟡 = Match final (potentiel)
- Couleurs : gradient représentant la progression du tournoi

---
