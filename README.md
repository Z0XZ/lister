# Lister

Vi har tidligere laget variabler som enten inneholder et tall eller en tekst (streng). Det finnes også andre måter å oppbevare data i en variabel på, og det vi skal se nærmere på her er hvordan vi kan lage, lagre og manipulere lister i Python.

## Lage en liste

For å lage en liste lager vi en variabel og tildeler den listen. En liste i Python kan inneholde både tall og tekst, og hvert element i listen skilles med et kommategn. Starten og slutten på listen rammes inn med firkantparenteser.
En liste kan altså se slik ut: [1, 3, 8, "hei", "hallo", 2901]

I Python kan man lage en liste og legge den inn i en variabel slik:

```Python
handleliste = ["Tomater", "Agurk", "Appelsin", "Sjokolade"]
```

I eksempelet over inneholder variabelen _handleliste_ en liste med 4 elementer.

## Hente ut fra listen

For å hente ut et bestemt element fra en liste kan vi ta utgangspunkt i navnet til variabelen for så å referere til nummeret som elementet har i listen. Når Python skal nummerere så begynner den på 0 og teller oppover. Element nummer 0 i listen over er altså "Tomater", mens element nummer 3 er "Sjokolade".

Om vi ønsker å referere til et element i listen kan vi gjøre det slik:

```Python
handleliste = ["Tomater", "Agurk", "Appelsin", "Sjokolade"]

print(hendleliste[2]) #printer ut "Appelsin"
```

I programmet over vil ordet _Appelsin_ skrives ut.

## Legge til i listen

Om vi ønsker å legge til noe til listen kan vi gjøre det også. Dette kan gjøres ved å bruke kommandoen _.append()_

I programmet under kan vi se hvordan man kan lage en tom liste og legge til elementer til listen.

```Python
liste = [] # Lager en liste som er tom

# Legger til elementer til listen. Det som står inne i parantesen er det som blir lagt til i lista:

liste.append(5)
liste.append("Hei")
liste.append(2022)

print(liste) # Skriver ut hele listen [5, "Hei", 2020]

```

## Regnemetoder med lister

#### Summen av verdiene i en liste

Vi kan bruke lister til å regne ut en del nyttig. Vi kan for eksempel finne summen av alle verdiene i en liste (om den bare består av tall):

```Python
liste1 = [1, 2, 3, 4] # Lager en liste med fire verdier

summen = sum(liste1) # Lagrer summen av tallene i listen til variabelen

print(summen) # Skriver ut 10
```

#### Telle antall elementer i en liste

Vi kan også telle hvor mange elementer det listen består av (f.eks. om vi ønsker å vite hvor mange tall det er i listen):

```Python
liste1 = [1, 2, 3, 4] # Lager en liste med fire verdier

antall_tall = len(liste1) # Lagrer antall tall i listen til variabelen

print(antall_tall) # Skriver ut 4 siden det er fire tall i listen
```

#### Regne ut gjennomsnitt

Dette kan vi også bruke til å regne ut f.eks. gjennomsnittet. Om vi deler summen vi fant i stad, med antall tall finner vi gjennomsnittet:

```Python
liste1 = [1, 2, 3, 4] # Lager en liste med fire verdier

summen = sum(liste1) # Lagrer summen av tallene i listen til variabelen
antall_tall = len(liste1) # Lagrer antall tall i listen til variabelen
gjennomsnitt = summen/antall_tall

print(gjennomsnitt) # Skriver ut 2.5 som er gjennomsnittet av verdiene i listen.
```

#### Telle antall verdier

Om vi vil finne ut hvor mange det er av en bestemt verdi kan vi gjøre dette ved å bruke .count()-metoden:

```Python
liste1 = [1, 1, 3, 4] # Lager en liste med fire verdier

antall1 = liste1.count(1) # Teller antall énere i listen og lagrer det i variabelen

print(antall1) # Skriver ut 2
```

#### Sortere verdiene i en liste

Vi kan sortere alle verdiene i en liste ved å bruke en metode som kalles for .sort() slik:

```Python
liste1 = [4, 1, 3, 4] # Lager en liste med fire verdier

liste1.sort() # Sorterer verdiene i listen

print(liste1) # Skriver ut [1, 1, 3, 4] som er den sorterte listen
```

## Oppgave

Du skal nå løse matematikkoppgavene under ved å bruke programmeringsmetodene vi har vist eksempler på over.

### Oppgave 2

Under ser du en liste med terningkast etter at man har kastet terning mange ganger:

```Python
terningkast = [3, 3, 5, 3, 6, 3, 1, 4, 4, 3, 5, 6, 5, 1, 6, 5, 3, 3, 1, 5, 2, 2, 2, 1, 5, 5, 5, 1, 1, 5, 3, 3, 3, 5, 5, 6, 4, 3, 3, 6, 2, 4, 4, 4, 6, 4, 4, 4, 1, 3, 4, 5, 2, 6, 5, 3, 5, 6, 6, 3, 3, 2, 6, 3, 1, 4, 4, 4, 6, 2, 2, 5, 2, 4, 6, 3, 3, 3, 4, 6, 4, 6, 1, 5, 2, 6, 2, 5, 4, 4, 5, 1, 5, 3, 5, 6, 4, 5, 5, 1, 2, 2, 3, 5, 5, 2, 4, 3, 4, 2, 5, 3, 6, 2, 5]
```

a) Kopier variabelen over.

b) Lag to nye variabler som inneholder summen av alle terningkastene og antall terningkast.

c) Regn ut gjennomsnittet av terningkastene og lagre dette i en ny variabel

d) Sorter listen, print den sorterte listen til skjermen og forsøk å finne medianen.

e) Få programmet til å telle alle verdiene i listen og skrive disse ut. Finn ut hva som er typetallet (det tallet det er flest av).
