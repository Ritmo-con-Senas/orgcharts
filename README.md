# Ritmo con Señas - Germany - Org-Charts

## Germany - Org-Charts
```mermaid
%%{init: {'theme':'forest'}}%%
flowchart TD
    rcs[(<b>Ritmo con Señas<br>Germany</b>
    <i>Nikolai von Krusenstiern</i><br>
    <a href="mailto:nikolai@ritmo-con-senas.de">nikolai@ritmo-con-senas.de</a>
    <a href="https://ritmo-con-senas.de" target="_blank">ritmo-con-senas.de</a>)]

    TUE[Tübingen<br>
    <b>KlangFolk e.V.</b><br>
    <a href="mailto:vorstand@klangfolk.de target="_blank"">vorstand@klangfolk.de</a>
    <a href="https://klangfolk.de" target="_blank">klangfolk.de</a>]

    DA[Darmstadt]
    
    B[Berlin]

    rcs -.-> TUE
    rcs -.-> DA
    rcs -.-> B

    TUE_MCS(<b>Música con Señas</b>
        <i>Cristóbal Araya Altamirano
        & Cédric Berner</i>
        weekly: 8-20<br>
        <a href="mailto:mcs@klangfolk.de" target="_blank">mcs@klangfolk.de</a>
        <a href="https://klangfolk.de/mcs" target="_blank">klangfolk.de/mcs</a>)

    TUE_MCS_2(<b>Música con Señas</b>
        <i>Nikolai von Krusenstiern</i>
        bi-weekly: 5-12<br>
        <a href="mailto:nikolai@ritmo-con-senas.de" target="_blank">nikolai@ritmo-con-senas.de</a>
        <a href="https://klangfolk.de/mcs" target="_blank">klangfolk.de/mcs</a>)
    
    TUE <--> TUE_MCS
    TUE <--> TUE_MCS_2

    DA_MCS(<b>Música con Señas</b>
        <i>Nikolai von Krusenstiern</i>
        monthly: 5-12<br>
        <a href="mailto:nikolai@ritmo-con-senas.de" target="_blank">nikolai@ritmo-con-senas.de</a>
        <a href="https://ritmo-con-senas.de/darmstadt" target="_blank">ritmo-con-senas.de/darmstadt</a>)

    DA --> DA_MCS

    B_P(<b>Percussion and Brass Band</b>
        <i>Bruno Abulafia</i>
        Concerts: monthly ?<br>
        <a href="mailto:bruno@ritmo-con-senas.de" target="_blank">bruno@ritmo-con-senas.de</a>
        <a href="https://ritmo-con-senas.de/berlin" target="_blank">ritmo-con-senas.de/berlin</a>)

    B_R(<b>Rixdorf con Señas</b>
        <i>Timm</i>
        Sessions: bi-monthly ?<br>
        <a href="mailto:rixdorfconsenas@posteo.de" target="_blank">rixdorfconsenas@posteo.de</a>
        <a href="https://ritmo-con-senas.de/berlin" target="_blank">ritmo-con-senas.de/berlin</a>)
    B --> B_P
    B --> B_R

%%    linkStyle 11 stroke-width:4px,stroke:blue

    classDef BLUE fill:lightblue
    classDef YEL fill:yellow
    classDef BLU fill:skyblue
    classDef ORA fill:orange

    class rcs,TUE_MCS,TUE_MCS_2,DA_MCS,B_P,B_R BLUE
    class x BLU
    class x YEL
    class TUE ORA

```

## KlangFolk e.V.

```mermaid
%%{init: {'theme':'forest'}}%%
flowchart TD
    E{Erasmus}

    TUE{Tübingen City}

    P{German<br>Project Fundings}

    TUE_LOC{Local Companies}
    
    KF(Tübingen<br><b>KlangFolk e.V.</b><br>
    Board:<br>- <i>Nikolai von Krusenstiern</i>,<br>- ...,<br>
    <a href="https://klangfolk.de" target="_blank">klangfolk.de</a>)

    TUE ==> |6k EUR<br>every Year| KF
    TUE_LOC --> KF
    P --> KF
    E -.-> |2025 ?| KF

    MCS["<b>Música con Señas</b><br>(Ritmo con Señas)"]
    TF["<b>Tü Folk Orchester</b><br>(Ethno)"]
    BF["<b>BalFolk</b><br>(BalFolk)"]

    KF <--> MCS
    KF <--> TF
    KF <--> BF

    MCS_1(Música con Señas<br>
        <i>Cristóbal Araya Altamirano 
        & Cédric Berner<i>)

    MCS_2(Música con Señas<br>
        <i>Nikolai von Krusenstiern</i>)    
    
    MCS --> MCS_1
    MCS --> MCS_2

%%    linkStyle 11 stroke-width:4px,stroke:blue

    classDef BLUE fill:lightblue
    classDef YEL fill:yellow
    classDef BLU fill:skyblue
    classDef ORA fill:orange

    class rcs,MCS_1,MCS_2,DA_MCS,B_P,B_R BLUE
    class x BLU
    class E,TUE,TUE_LOC,P YEL
    class KF ORA
```


(c) 2024 Nikolai von Krusenstiern
