# Algorytmy ocen zawodników

## 🥅 Napastnik — V4

### Baza
6,75

### Gole — liczba
+ 0,06 × gole  
maksymalnie +1,44

### Gole / 100 minut
+0,35 × min(1, gole/15) × min(1, G/100 ÷ 2,5)

### Skuteczność
+0,005 × (skuteczność − 40)  
limit −0,15 / +0,15

### Asysty
+0,025 × asysty  
maksymalnie +0,50

+0,08 × min(1, asysty/8) × min(1, A/100 ÷ 1,5)

### Kluczowe podania
+0,01 × KP  
maksymalnie +0,30

+0,03 × min(1, KP/20) × min(1, KP/100 ÷ 3)

### DefCons − straty
D = (DefCons − straty) / minuty × 100

+0,015 × D  
limit −0,30 / +0,30

### Wyniki zespołu
0,10 × [(W + 0,5R − P) / mecze]

+0,02 × [(pogromy − blamaże) / mecze]

### Kary
−0,03 × liczba kar 2-minutowych


---

# 🏃 Skrzydłowy — V2

### Baza
6,75

### Gole
+0,045 × gole  
maksymalnie +0,90

+ bonus za tempo goli

### Skuteczność
+0,0035 × (skuteczność − 40)  
limit −0,10 / +0,10

### Asysty
+0,04 × asysty  
maksymalnie +0,80

+ bonus za tempo asyst

### Kluczowe podania
+0,015 × KP  
maksymalnie +0,60

+ bonus za tempo KP

### DefCons − straty
D = (DefCons − straty) / minuty × 100

+0,035 × D  
limit −0,50 / +0,50

### CS i gole stracone
+0,10 × (CS / mecze)

+0,10 × (1,5 − gole stracone/mecz)  
limit ±0,10

### Wyniki
0,10 × [(W + 0,5R − P) / mecze]

+0,02 × [(pogromy − blamaże) / mecze]

### Kary
−0,03 × liczba kar 2-minutowych


---

# 🛡️ Obrońca — V1

### Baza
6,75

### DefCons − straty
D = (DefCons − straty) / minuty × 100

+0,12 × D  
limit −0,60 / +0,60

### Czyste konta
+0,60 × (CS / mecze zawodnika)

### Gole stracone przez drużynę
+0,40 × (1,5 − gole stracone/mecz)  
limit −0,40 / +0,40

### Gole
+0,05 × gole  
maksymalnie +0,50

### Asysty
+0,035 × asysty  
maksymalnie +0,35

### Kluczowe podania
+0,008 × KP  
maksymalnie +0,20

### Wyniki
0,15 × [(W + 0,5R − P) / mecze]

+0,03 × [(pogromy − blamaże) / mecze]

### Kary
−0,03 × liczba kar 2-minutowych


---

# 🧤 Bramkarz — V1

### Baza
6,50

### Skuteczność interwencji

interwencje = strzały na bramkę − gole stracone

skuteczność = interwencje / strzały × 100

bonus = (skuteczność − 70) × 0,025

limit −0,75 / +0,75

### Gole stracone
(1,00 − gole/mecz) × 0,50

limit −0,50 / +0,50

### Czyste konta
+0,60 × (CS / mecze)

### Wyniki
0,15 × [(W + 0,5R − P) / mecze]

+0,03 × [(pogromy − blamaże) / mecze]

### Kary
−0,03 × liczba kar 2-minutowych


---

# 🩹 Faule, kary i kontuzje

## Faule

faule/mecz = (100 − średnie posiadanie) / 3

## Kary 2-minutowe

kary/mecz = faule/mecz ÷ 20 + gole stracone/mecz ÷ 3

## Wpływ kar na ocenę

−0,03 za każdą karę 2-minutową

## Kontuzje

60 kontuzji na całą ligę.

Losowanie:

- bramkarze — 1 los
- obrońcy — 2 losy
- skrzydłowi — 4 losy
- napastnicy — 4 losy

Ofensywny zawodnik planowany powyżej 30 min/mecz otrzymuje dodatkowy los.

## Osłabienie drużyny przez kontuzje

2+ ofensywnych, w tym 1 podstawowy → −1 ATK

Podstawowy bramkarz → −1 DEF

2+ obrońców, w tym 1 podstawowy → −1 DEF