---
layout: page
title: "Kod för prog pass1 grupp1 MaProgTjej19"
---

[Här finns slides för föreläsningen](https://docs.google.com/presentation/d/1cny5LYP0HtL2TGslr_ZBUxCxvYSomZDTQLzeh7Ap5S0/edit?usp=sharing).

I prompten kan vi testa att exekvera en rad i taget:
```
> print('Hej')
Hej
> print('Välkommen!')
Välkommen!
```
## Matematiska operationer
Matematiska operationer i prompten fungerar som en miniräknare:

```
> 2 + 3
5

> x = 2 + 7
> print(x)
9
> x
9

> 9 / 2
4.5

> 9 // 2
4

> 9 % 2
1
```
## Variabler

Variabler räknar ut högerled först och sen sparar värdet av uträkningen i variabelnamnet.

```
> a = 10
> b = a
> a = 3
> print(b)
10

> x = 2 ** 3
> y = 3 * x
> y
24
```

Bool-variabler är sanna eller falska
```
> 9 / 3 == 3
True
> 9 % 2 == 0
False
```
## Input och printa output

Öppna en fil och skriv programmet i den.

För att läsa in text från användaren:
```python
print('Vad heter du?')
name = input()
print('Hej', name)
```
i promten:
```
Vad heter du?
```
Skriv in ditt namn och tryck enter (ny rad) och då svarar programmet:
```
Hej ___
```

### Omvandlingar mellan datatyper

All input tolkas som textsträngar, så om vi vill räkna med det behöver vi omvändla texten till tal med int():

```python
text = input()
tal = int(text)
print(tal ** 2)
```

I promten väntar programmet på att du ska mata in ett tal och trycka enter och sen skriver det ut talet i kvadrat.

Vi kan göra om tal till textsträngar med hjälp av str(*vårt tal*).

Vi kan slå samman textsträngar med hjälp av plustecken 'Hej ' + 'på dig' blir 'Hej på dig'.

Så då kan vi slå ihop text och tal med plus och den omvandlade strängen av talet 'Hej ' + str(*vårt tal*)
```pyhton
tal = int(input())
print('Hej ' + str(tal))
```

Inuti str() kan en hel uträkning finnas, t ex kan den skriva ut kvadraten på talet vi matat in:
```python
tal = int(input())
print('Kvadrat ' + str(tal**2))
```

## Övningar
#### Övning 1: 
Tänk att vi har ett hemligt lösenord, typ “Nicole”
Om användaren till vårt program skriver in rätt lösenord, skriv “Välkommen”.
Annars skriv “Fel lösenord”

```python
pw = input()
if pw == 'Nicole':
    print('Välkommen')
elif pw == 'Hej':
    print('Hej på dig')
else:
    print('Fel lösenord!')
```

#### Övning 2:
Skriv ett program som tar en persons födelseår samt dess ålder som indata och skriver ut “Grattis i efterskott” om den redan har fyllt år och “Grattis i förskott” annars.
```python
print('Vilket år är du född?')
born = int(input())
print('Hur gammal är du?')
age = int(input())
if 2019 == age + born:
    print('Grattis i efterskott')
else:
    print('Grattis i förskott')
```
Om personen har fyllt år i år (2019) är summan av dess ålder och födelseår exakt 2019. Notera att vi litar på att användaren matar in riktiga värden. Om personen fyller år idag säger vi `'Grattis i efterskott'`.

