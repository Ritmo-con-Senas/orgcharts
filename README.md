# Ritmo con Señas - Germany - Org-Charts

## Germany - Org-Charts
```mermaid
%%{init: {'theme':'forest'}}%%
flowchart TD
    rcs[(<b>Ritmo con Señas<br>Germany</b>
    <i>Nikolai von Krusenstiern</i><br>
    <a href>nikolai@ritmo-con-senas.de</a>
    <a href>ritmo-con-senas.de</a>)]

    TUE[Tübingen<br>
    <b>KlangFolk e.V.</b><br>
    <a href>vorstand@klangfolk.de</a>
    <a href>klangfolk.de</a>]

    DA[Darmstadt]
    
    B[Berlin]

    rcs -.-> TUE
    rcs -.-> DA
    rcs -.-> B

    TUE_MCS(<b>Música con Señas</b>
        <i>Cristóbal Araya Altamirano
        & Cédric Berner</i>
        weekly: 8-20<br>
        <a href>mcs@klangfolk.de</a>
        <a href>klangfolk.de/mcs</a>)

    TUE_MCS_2(<b>Música con Señas</b>
        <i>Nikolai von Krusenstiern</i>
        bi-weekly: 5-12<br>
        <a href>nikolai@ritmo-con-senas.de</a>
        <a href>klangfolk.de/mcs</a>)
    
    TUE <--> TUE_MCS
    TUE <--> TUE_MCS_2

    DA_MCS(<b>Música con Señas</b>
        <i>Nikolai von Krusenstiern</i>
        monthly: 5-12<br>
        <a href>nikolai@ritmo-con-senas.de</a>
        <a href>ritmo-con-senas.de/darmstadt</a>)

    DA --> DA_MCS

    B_P(<b>Percussion and Brass Band</b>
        <i>Bruno Abulafia</i>
        Concerts: monthly ?<br>
        <a href>bruno@ritmo-con-senas.de</a>
        <a href>ritmo-con-senas.de/berlin</a>)

    B_R(<b>Rixdorf con Señas</b>
        <i>Timm</i>
        Sessions: bi-monthly ?<br>
        <a href>rixdorfconsenas@posteo.de</a>
        <a href>ritmo-con-senas.de/berlin</a>)
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

    P{German Project Fundings}

    TUE_LOC{Local Companies}
    
    KF(Tübingen<br>KlangFolk e.V.<br>
    Board:<br>- Nikolai von Krusenstiern,<br>- ...,<br>
    klangfolk.de)

    TUE ==> |6k EUR<br>every Year| KF
    TUE_LOC --> KF
    P --> KF
    E -.-> |2025 ?| KF

    MCS["Música con Señas<br>(Ritmo con Señas)"]
    TF["Tü Folk Orchester<br>(Ethno)"]
    BF["BalFolk<br>(BalFolk)"]

    KF <--> MCS
    KF <--> TF
    KF <--> BF

    MCS_1(Música con Señas<br>
        Cristóbal Araya Altamirano & Cédric Berner)

    MCS_2(Música con Señas<br>
        Nikolai von Krusenstiern)    
    
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
