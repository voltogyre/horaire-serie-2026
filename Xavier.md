# horaire-serie-2026
# 🏒 Tournoi Séries 2026 - Chemins de Dépendances
## 🔵 HUSKY 4 (m18b) - Xavier

### Structure des Dépendances

```mermaid
graph TD
    M18B05["✌️ MATCH 05<br/>Alliés 2 (1) @ HUSKY 4 (6)<br/>(21 mars 17:30)<br/>St-Étienne"]
    M18B20["✌️ MATCH 20<br/>SEIGNEURS 1 (2) @ HUSKY 4 (6)<br/>(28 mars 20:30)<br/>Lévis"] 
    M18B30[Rapides 2 vs Sénateurs 1<br/>Seigneurs 3 vs Alliés 1]
    M18B31[Éclaireurs2 vs Commandeurs 3<br/>Seigneurs 1 vs Rapides 1<br/>Perdant entre Commandeurs 2 vs Éclaireurs 3]
    M18B28[Commandeurs 2 vs Éclaireurs 3]
   
    M18B27["🔴 MATCH 27<br/>HUSKY 1 @ HUSKY 4<br/>(4 avril 14:00)<br/>Montmagny"]
    M18B27 -->|Gagnant| M18B33["MATCH 33<br/>Gagnant #27<br/>(11 avril 12:30)<br/>Saint-Damien-de-Buckland"]
    M18B33 -->|Gagnant| M18B36["🟡 MATCH 36<br/>FINALE<br/>(12 avril 15:30)<br/>Saint-Isidore"]
    M18B32 -->|Gagnant| M18B34["MATCH 34<br/>Gagnant #32<br/>(11 avril 15:00)<br/>Sainte-Claire"]
    M18B34 -->|Gagnant| M18B35["MATCH 35<br/>Perdant #33/Gagnant #34<br/>(11 avril 20:00)<br/>Sainte-Claire"]
    M18B35 -->|Gagnant| M18B36
    M18B27 -->|Gagnant| W["Régionnaux"]
    M18B34 -->|Gagnant| W
    M18B27 -->|Perdant| M18B32["MATCH 32<br/>Perdant #27<br/>(5 avril 16:00)<br/>Saint-Agapit"]
    M18B33 -->|Perdant| M18B35
    M18B34 -->|Perdant| K["Fin de la saison"]
    M18B30 -->|Compétition| M18B32
    M18B31 -->|Compétition| M18B34
    M18B28 -->|Compétition| M18B33
    M18B28 -->|Compétition| M18B31
    
    linkStyle 0,1,2,3,4,5,6 stroke:#22c55e,stroke-width:2.5px
    linkStyle 7,8,9 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    linkStyle 10,11,12,13 stroke:##1b75be,stroke-width:1.5px,stroke-dasharray: 2 1
    


```
sans la compétition
```mermaid
graph TD
    M18B05["✌️ MATCH 05<br/>Alliés 2 (1) @ HUSKY 4 (6)<br/>(21 mars 17:30)<br/>St-Étienne"]
    M18B20["✌️ MATCH 20<br/>SEIGNEURS 1 (2) @ HUSKY 4 (6)<br/>(28 mars 20:30)<br/>Lévis"] 
    
    M18B27["🔴 MATCH 27<br/>HUSKY 1 @ HUSKY 4<br/>(4 avril 14:00)<br/>Montmagny"]
    M18B27 -->|Gagnant| M18B33["MATCH 33<br/>Gagnant #27<br/>(11 avril 12:30)<br/>Saint-Damien-de-Buckland"]
    M18B33 -->|Gagnant| M18B36["🟡 MATCH 36<br/>FINALE<br/>(12 avril 15:30)<br/>Saint-Isidore"]
    M18B32 -->|Gagnant| M18B34["MATCH 34<br/>Gagnant #32<br/>(11 avril 15:00)<br/>Sainte-Claire"]
    M18B34 -->|Gagnant| M18B35["MATCH 35<br/>Perdant #33/Gagnant #34<br/>(11 avril 20:00)<br/>Sainte-Claire"]
    M18B35 -->|Gagnant| M18B36
    M18B27 -->|Gagnant| W["Régionnaux"]
    M18B34 -->|Gagnant| W
    M18B27 -->|Perdant| M18B32["MATCH 32<br/>Perdant #27<br/>(5 avril 16:00)<br/>Saint-Agapit"]
    M18B33 -->|Perdant| M18B35
    M18B34 -->|Perdant| K["Fin de la saison"]
    
    linkStyle 0,1,2,3,4,5,6 stroke:#22c55e,stroke-width:2.5px
    linkStyle 7,8,9 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    


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

