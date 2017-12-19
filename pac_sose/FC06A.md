# SOSE: FC06A Comuni - Funzioni nel Settore Sociale (al netto del servizio di Asilo Nido) - Fabbisogni, caratteristiche e prestazioni

## Descrizione del dataset


**Tipo di dataset:** standard/ordinary?

**Tipo di flusso:** batch

**Tipo di file:** CSV

**Scheda:** 

**Modalità di ingestion su DAF:** scarico su SFTP


## Elementi

| Nome | Tipo   | Descrizione                     |
|------|--------|---------------------------------|
| ANNO | number | Anno di analisi  |
| COMUNE_CAT_COD | string  | codice catastale del comune |
| CAT_DET_COD_1 |  | Popolazione residente
| CAT_DET_COD_2 |  | Economia locale
| CAT_DET_COD_3 |  | Prezzi degli input
| CAT_DET_COD_4 |  | Scelte organizzative
| CAT_DET_COD_5 |  | Disagio sociale
| CAT_DET_COD_6 |  | Demografia
| COEFF_TEORICO |  | Coefficiente di Fabbisogno Standard per il Comune |
| IND1 |  | Spesa storica del servizio sociale per abitante(€)
| IND3 |  | Spesa storica vs fabbisogno standard(%)
| IND4 |  | Livello servizi offerti vs livello servizi standard(%)
| IND5 |  | Spesa del servizio sociale per utente (€)
| IND6 |  | Utenti che usufruiscono del servizio sociale(%)
| IND7 |  | Ore annue di assistenza per utente(h)
| IND8 |  | Ore di apertura settimanale al pubblico degli sportelli(h)
| LQP_COD_1 |  | Differenza tra spesa storica e fabbisogno standard in % rispetto al fabbisogno standard |
| LQP_COD_2 |  | Differenza tra livello dei servizi storico e livello dei servizi standard in % rispetto al livello dei servizi standard |
| LQP_COD_3 |  | Flag Comune non valutabile |
| LQP_COD_4 |  | Flag percentile anomalo (differenza % minore del 5^ percentile o maggiore del 95^ percentile) |
| LQP_COD_5 |  | Posizione del Comune rispetto alla spesa |
| LQP_COD_6 |  | Posizione del Comune rispetto al livello dei servizi |
| LQP_COD_S |  | Misura (da 0 a 10) della capacità del Comune di soddisfare la domanda di servizi espressa dai cittadini, tenendo conto della spesa e dei servizi offerti rispetto allo standard |


## Esempio del flusso

```
"ANNO";"COMUNE_CAT_COD";"CAT_DET_COD_1";"CAT_DET_COD_2";"CAT_DET_COD_3";"CAT_DET_COD_4";"CAT_DET_COD_5";"CAT_DET_COD_6";"COEFF_TEORICO";"IND1";"IND3";"IND4";"IND5";"IND6";"IND7";"IND8";"LQP_COD_1";"LQP_COD_2";"LQP_COD_3";"LQP_COD_4";"LQP_COD_5";"LQP_COD_6";"LQP_COD_S"
"2010";"A052";"0.241198659";"0.18759529";"0.140769629";"0.125286548";"0.07381511";"0.231334763";"0.000372432";"45.44891008";"-46.33146032";"12.65132342";"498.434365";"9.118333982";"24.34123223";"22";"-46.33146032";"12.65132342";"0";"0";"2";"7";"7.8"
"2010";"A146";"0";"0.234508916";"0.128945838";"0.26506458";"-0.061173493";"0.432654159";"4.21282E-06";"19.03405573";"-68.77162557";"1.618902243";"100.7868852";"18.88544892";"0";"0";"-68.77162557";"1.618902243";"0";"0";"1";"6";"7.6"
"2010";"A182";"0.401038042";"0.163720797";"0.09309391";"0.15224944";"0.023792772";"0.166105039";"0.002151788";"8.050582265";"-92.3963627";"-24.20842532";"53.71617254";"14.98725967";"91.95134062";"25";"-92.3963627";"-24.20842532";"0";"1";"1";"3";"5.8"
"2010";"A189";"0";"0.306087138";"0.165627329";"0.134367307";"0.023202864";"0.370715361";"8.59804E-06";"25.75129534";"-50.52269835";"-53.69759968";"1656.666667";"1.554404145";"0";"0";"-50.52269835";"-53.69759968";"0";"0";"2";"1";"4.2"
"2010";"A197";"0";"0.237909465";"0.135197783";"0.253890896";"0.060888409";"0.312113447";"1.06398E-05";"33.29577465";"-47.70077142";"-11.20408468";"963.1111111";"3.457106274";"0";"0";"-47.70077142";"-11.20408468";"0";"0";"2";"4";"6"
"2010";"A211";"0";"0.322474841";"0.154728108";"0.18441521";"0.005696277";"0.332685563";"1.17486E-05";"5.196754564";"-90.66717241";"-37.85033281";"";"0";"";"0";"-90.66717241";"-37.85033281";"0";"1";"1";"2";"5.2"
"2010";"A227";"0";"0.255219955";"0.148698709";"0.235247741";"-0.006600813";"0.367434408";"5.76903E-06";"10.66205534";"-79.9885855";"-23.54435458";"";"0";"";"0";"-79.9885855";"-23.54435458";"0";"1";"1";"3";"5.8"
"2010";"A245";"0";"0.243374902";"0.110390779";"0.22580312";"0.164255444";"0.256175755";"5.81645E-06";"31.3683224";"-56.14633701";"-12.13592844";"";"0";"";"0";"-56.14633701";"-12.13592844";"0";"0";"2";"4";"6"
"2010";"A436";"0.093471206";"0.234260617";"0.150935552";"0.170160412";"0.055154045";"0.296018167";"8.36766E-05";"48.66357827";"-22.09541998";"-0.419193864";"603.2356436";"8.067092652";"0";"11";"-22.09541998";"-0.419193864";"0";"0";"4";"5";"5.8"
"2010";"A523";"0";"0.201317917";"0.130762624";"0.260830531";"0.033941396";"0.373147532";"3.95247E-06";"27.12080537";"-56.24379501";"19.52563892";"384.8571429";"7.046979866";"180";"19";"-56.24379501";"19.52563892";"0";"0";"2";"7";"7.8"
"2010";"A605";"0";"0.290698192";"0.131924247";"0.19826885";"0.055909585";"0.323199126";"1.92409E-05";"11.13342697";"-82.36800338";"19.4565016";"259.9016393";"4.283707865";"0";"27";"-82.36800338";"19.4565016";"0";"1";"1";"7";"8.2"
"2010";"A689";"0";"0.280626344";"0.17258253";"0.279851749";"-0.016902709";"0.283842087";"2.61273E-05";"35.08045433";"-39.29027327";"-30.5628148";"451.9817073";"7.761476574";"0";"13";"-39.29027327";"-30.5628148";"0";"0";"3";"3";"5"
"2010";"A708";"0";"0.268534956";"0.171125311";"0.282112839";"0.002108339";"0.276118555";"2.17419E-05";"25.69187359";"-55.19249363";"15.06782124";"1896.916667";"1.354401806";"0";"0";"-55.19249363";"15.06782124";"0";"0";"2";"7";"7.8"
"2010";"A738";"0";"0.289100508";"0.15471698";"0.310159759";"-0.076698465";"0.322721218";"5.58924E-06";"45.31337325";"-13.08396922";"-42.45501359";"";"0";"";"27";"-13.08396922";"-42.45501359";"0";"0";"5";"2";"3.6"
"2010";"A793";"0.014937442";"0.263954946";"0.13775474";"0.2597798";"0.006153016";"0.317420055";"1.03869E-05";"46.81131003";"-24.77763454";"-36.61891699";"50.15497503";"20.68769537";"24.59090909";"36";"-24.77763454";"-36.61891699";"0";"0";"4";"2";"4"
"2010";"A813";"0";"0.213289193";"0.148866903";"0.06900905";"0.312849483";"0.255985372";"1.92415E-06";"23.82941176";"";"";"";"0";"";"0";"";"";"2";"0";"";"";""
"2010";"A889";"0";"0.272444582";"0.170304741";"0.145898104";"0.036266815";"0.375085759";"1.9954E-05";"21.23302469";"-55.73442379";"-14.3924984";"1031.925";"2.057613169";"0";"0";"-55.73442379";"-14.3924984";"0";"0";"2";"4";"6"
"2010";"A998";"0";"0.257291581";"0.160965233";"0.287448124";"-0.036034516";"0.330329579";"2.41832E-05";"23.88451966";"-57.54081619";"-18.75831679";"448.4485981";"5.326032852";"0";"0";"-57.54081619";"-18.75831679";"0";"0";"2";"4";"6"

```
