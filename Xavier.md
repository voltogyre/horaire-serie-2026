# horaire-serie-2026
# 🏒 Tournoi Séries 2026 - Chemins de Dépendances
## 🔵 HUSKY 4 (m18b) - Xavier

### Structure des Dépendances

```mermaid
graph TD
    A["🔴 MATCH 20<br/>SEIGNEURS 1 @ HUSKY 4<br/>(28 mars 20:30)<br/>Lévis"] 
    
    A -->|Gagnant| B["MATCH 27<br/>Gagnant #20<br/>(4 avril 14:00)<br/>Montmagny"]
    A -->|Perdant| C["MATCH 24<br/>Perdant #20<br/>(29 mars 11:30)<br/>Sainte-Claire"]
    
    B -->|Gagnant| D["MATCH 33<br/>Gagnant #27<br/>(11 avril 12:30)<br/>Saint-Damien-de-Buckland"]
    B -->|Perdant| E["MATCH 32<br/>Perdant #27<br/>(5 avril 16:00)<br/>Saint-Agapit"]
    
    C -->|Gagnant| F["MATCH 29<br/>Gagnant #24<br/>(4 avril 18:45)<br/>Saint-Isidore"]
    
    D -->|Gagnant| I["🟡 MATCH 36<br/>FINALE<br/>(12 avril 15:30)<br/>Saint-Isidore"]
    D -->|Perdant| J["MATCH 35<br/>Perdant #33<br/>(11 avril 20:00)<br/>Sainte-Claire"]
    
    E -->|Gagnant| H["MATCH 34<br/>Gagnant #32<br/>(11 avril 15:00)<br/>Sainte-Claire"]
    
    F -->|Gagnant| G["MATCH 31<br/>Gagnant #29<br/>(5 avril 14:30)<br/>Saint-Agapit"]
    
    G -->|Gagnant| H
    
    H -->|Gagnant| J
    
    J -->|Gagnant| I
    
    C -->|Perdant| K["Fin de la saison"]
    F -->|Perdant| K["Fin de la saison"]
    G -->|Perdant| K["Fin de la saison"]
    H -->|Perdant| K["Fin de la saison"]
    B -->|Gagnant| L["Régionnaux"]
    H -->|Gagnant| L["Régionnaux"]

    linkStyle 0,2,4,5,7,8,9,10,11,16,17 stroke:#22c55e,stroke-width:2.5px
    linkStyle 1,3,6,12,13,14,15 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    

```

### 📍 Chemins Vers la FINALE (Match 36)

| Match | Chemins Possibles | Nombre de Chemins |
|-------|-------------------|-------------------|
| **20** | DIRECT | 1 |
| **27** | W20 | 1 |
| **24** | L20 | 1 |
| **32** | W20 → L27 | 1 |
| **33** | W20 → W27 | 1 |
| **29** | L20 → W24 | 1 |
| **34** | L20 → W24 → W29 → W31 **OU** W20 → L27 → W32 | 2 |
| **31** | L20 → W24 → W29 | 1 |
| **35** | L20 → W24 → W29 → W31 → W34 **OU** W20 → L27 → W32 → W34 **OU** W20 → W27 → L33 | 3 |
| **36** | L20 → W24 → W29 → W31 → W34 → W35 **OU** W20 → L27 → W32 → W34 → W35 **OU** W20 → W27 → L33 → W35 **OU** W20 → W27 → W33 | 4 |

---

## 🔑 Légende

- **W#** = Gagnant du match #
- **L#** = Perdant du match #
- **OU** = Chemin alternatif possible
- 🔴 = Match initial (garantis)
- 🟡 = Match final (potentiel)
- Couleurs : gradient représentant la progression du tournoi

