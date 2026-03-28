# horaire-serie-2026
# 🏒 Tournoi Séries 2026 - Chemins de Dépendances

## 📊 Résumé

Ce document visualise graphiquement les chemins possibles que les équipes **Husky 4 (Xavier)** et **Husky 1 (Gabriel)** peuvent emprunter lors du tournoi.

---

## 🔵 HUSKY 4 (m18b) - Xavier

### Structure des Dépendances

```mermaid
graph TD
    M18B05["✌️ MATCH 05<br/>Alliés 2 (1) @ HUSKY 4 (6)<br/>(21 mars 17:30)<br/>St-Étienne"]
    M18B20["✌️ MATCH 20<br/>SEIGNEURS 1 @ HUSKY 4<br/>(28 mars 20:30)<br/>Lévis"] 
    
    M18B27["🔴 MATCH 27<br/>Gagnant #20<br/>(4 avril 14:00)<br/>Montmagny"]
    M18B27 -->|Gagnant| M18B33["MATCH 33<br/>Gagnant #27<br/>(11 avril 12:30)<br/>Saint-Damien-de-Buckland"]
    M18B27 -->|Perdant| M18B32["MATCH 32<br/>Perdant #27<br/>(5 avril 16:00)<br/>Saint-Agapit"]
    M18B33 -->|Gagnant| M18B36["🟡 MATCH 36<br/>FINALE<br/>(12 avril 15:30)<br/>Saint-Isidore"]
    M18B33 -->|Perdant| M18B35["MATCH 35<br/>Perdant #33<br/>(11 avril 20:00)<br/>Sainte-Claire"]
    M18B32 -->|Gagnant| M18B34["MATCH 34<br/>Gagnant #32<br/>(11 avril 15:00)<br/>Sainte-Claire"]
    M18B34 -->|Gagnant| M18B35
    M18B35 -->|Gagnant| M18B36
    M18B34 -->|Perdant| K["Fin de la saison"]
    M18B27 -->|Gagnant| W["Régionnaux"]
    M18B34 -->|Gagnant| W["Régionnaux"]

    linkStyle 0,2,4,5,6,8,9 stroke:#22c55e,stroke-width:2.5px
    linkStyle 1,3,7 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    

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

## 🟣 HUSKY 1 (m21c) - Gabriel

### Structure des Dépendances

```mermaid
graph TD
    A["🔴 MATCH 7<br/>HUSKY 1 @ SEIGNEURS 2<br/>(28 mars 16:00)<br/>Lévis"] 
    
    A -->|Gagnant| B["MATCH 14<br/>Gagnant #7<br/>(4 avril 19:45)<br/>Saint-Romuald"]
    A -->|Perdant| C["MATCH 10<br/>Perdant #7<br/>(29 mars 19:00)<br/>Saint-Nicolas"]
    
    B -->|Gagnant| D["MATCH 17<br/>Gagnant #14<br/>(11 avril 14:30)<br/>Lévis"]
    B -->|Perdant| E["MATCH 16<br/>Perdant #14<br/>(5 avril 17:30)<br/>Sainte-Marie"]
    
    C -->|Gagnant| F["MATCH 12<br/>Gagnant #10<br/>(4 avril 18:00)<br/>Saint-Agapit"]
    
    D -->|Gagnant| I["🟡 MATCH 20<br/>FINALE<br/>(12 avril 11:30)<br/>Saint-Agapit"]
    
    F -->|Gagnant| G["MATCH 15<br/>Gagnant #12<br/>(5 avril 16:00)<br/>Sainte-Marie"]
    
    E -->|Gagnant| H["MATCH 18<br/>Gagnant #16<br/>(11 avril 16:00)<br/>Lévis"]
    
    G -->|Gagnant| H
    
    H -->|Gagnant| J["MATCH 19<br/>Gagnant #18<br/>(11 avril 20:30)<br/>Lévis"]
    
    D -->|Perdant| J
    
    J -->|Gagnant| I
    C -->|Perdant| K["Fin de la saison"]
    F -->|Perdant| K["Fin de la saison"]
    G -->|Perdant| K["Fin de la saison"]
    E -->|Perdant| K["Fin de la saison"]
    J -->|Perdant| K["Fin de la saison"]
    B -->|Gagnant| L["Régionnaux"]
    H -->|Gagnant| L["Régionnaux"]

    linkStyle 0,2,4,5,6,7,8,9,11,17,18 stroke:#22c55e,stroke-width:2.5px
    linkStyle 1,3,10,12,13,14,15,16 stroke:#ef4444,stroke-width:2.5px,stroke-dasharray:6 4
    

```

### 📍 Chemins Vers la FINALE (Match 20)

| Match | Chemins Possibles | Nombre de Chemins |
|-------|-------------------|-------------------|
| **7** | DIRECT | 1 |
| **10** | L7 | 1 |
| **14** | W7 | 1 |
| **12** | L7 → W10 | 1 |
| **16** | W7 → L14 | 1 |
| **15** | L7 → W10 → W12 | 1 |
| **17** | W7 → W14 | 1 |
| **18** | L7 → W10 → W12 → W15 **OU** W7 → L14 → W16 | 2 |
| **19** | L7 → W10 → W12 → W15 → W18 **OU** W7 → L14 → W16 → W18 **OU** W7 → W14 → L17 | 3 |
| **20** | L7 → W10 → W12 → W15 → W18 → W19 **OU** W7 → L14 → W16 → W18 → W19 **OU** W7 → W14 → L17 → W19 **OU** W7 → W14 → W17 | 4 |

---

## 📈 Statistiques

### Densité de Chemins

| Équipe | Match Initial | Match Final | Chemins à la Finale |
|---------|---------------|-------------|-------------------|
| **Husky 4** | Match 20 | Match 36 | 4 chemins |
| **Husky 1** | Match 7 | Match 20 | 4 chemins |

### Profondeur du Tournoi

| Équipe | Profondeur Max (victoires/défaites) | Nombre de Matches |
|--------|-------------------------------------|------------------|
| **Husky 4** | 5 niveaux (W20→W27→W33→W35→W36) | 10 matches |
| **Husky 1** | 5 niveaux (L7→W10→W12→W15→W18→W19) | 10 matches |

---

## 🔑 Légende

- **W#** = Gagnant du match #
- **L#** = Perdant du match #
- **OU** = Chemin alternatif possible
- 🔴 = Match initial (garantis)
- 🟡 = Match final (potentiel)
- Couleurs : gradient représentant la progression du tournoi

---

## 💡 Interprétation

### Pour Xavier (Husky 4)
- **Scénario le plus court**: Gagner en match 20 → Gagner en match 27 → ... → 4 victoires jusqu'à la finale
- **Scénario alternatif**: Perdre en match 20 → Gagner en matches 24, 29, 31 → ... → 4 victoires jusqu'à la finale
- **Flexibilité**: 4 chemins différents possibles pour atteindre la finale (match 36)

### Pour Gabriel (Husky 1)
- **Scénario optimal**: Gagner en match 7 → Gagner en match 14 → ... → 4 victoires jusqu'à la finale
- **Scénario alternatif**: Perdre en match 7 → Gagner en matches 10, 12, 15 → ... → 4 victoires jusqu'à la finale
- **Flexibilité**: 4 chemins différents possibles pour atteindre la finale (match 20)

---

