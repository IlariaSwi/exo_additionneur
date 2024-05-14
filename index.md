---
title: "GYAPI - Exercices additionneur"
permalink: /
layout: default
---

# Additionneur - Exercices

## Question 1

Avec l’additionneur ci-dessus, est-il possible d’obtenir des 1 sur toutes les sorties, donc d’avoir S<sub>2</sub> = S<sub>1</sub> = S<sub>0</sub> = 1?

<iframe style="width: 100%; height: 360px; border: 0" src="https://logic.modulo-info.ch/?mode=tryout&data=N4NwXAbANAxg9gWwA5wHYFNUBcDOZgCWqADPlgJ5LpgDkRNUKeA2gIwCcxUAHAKwC6UOACcCmLLRwMCAEzBdUAQwTUaAQVY0AvlCKsylVfUZwWAJk48BQ0eMnS5rKEpW01xbbtRmDVWsaYwZjMAZi5WM2sRMWx7XTkzZ2VVACFNHSIQ3yNUBkDmELCoCKjbWJopeLAQpNcaFI8dRRkZdGFSYAo-GmbW4TzTIJDWLjNiayJabgBaEYY4AFcJNicI-iaWtv1Ow1petoHzEagxidRaVhDZ3nmloNZoVgB2daEljq7VRaxDoeOzJ6lGISCoOMCsbi1VQAZUabyw20+tG+v2C-0BgmidlBVQ4UNo0PS8J8O26KJMLFYrF4JwxNmBcVkYDG+Jo0LM2h0AHcCMJ0Cw2IlqYIVsVuCKHsV2BKnidiCKatKoMFigAWCU8EXhEL8dZAA"></iframe>

## Exercice 1

- En connectant des additionneurs complets, réalisez un circuit qui additionne deux nombres `A` et `B` de quatre bits, numérotés `A0` à `A3` et `B0` à `B3`, respectivement. Combien de bits de sortie doit-il y avoir pour traiter toutes les valeurs possibles ?
- Les entrées sont déjà disposées. Glissez autant d’additionneurs et de bits de sortie que nécessaire et connectez les composants du circuit.


<iframe style="width: 150%; height: 530px; border: 0" src="https://logic.modulo-info.ch/?mode=full&showonly=out,adder&data=N4NwXAbANA9gDgFwM5mAXygYxgWzjAOwFMDlUBLAgBlQQE84iwByS5qfFAbQE4qoALFQC6sAE7kSCFknbkAJmADMUAgEMcTZgEElzDJQCMtBlrYcY3Q30Ejxk0jLmL+6zS20AmfVEqeTjCzmnGBcnjZCojASUk6+ioaqGlrahj6USgFmBOwhXEoRdtEO0syy8WCeSe46VOkEAllBORZWSvx8UTGOZc5ghgCs1VoAQnoGBANNrC15nu1QnfaxvRWGAsMsI94TENPBlqFKC0vFK+UK-Spuo2kTAOz7s4dcAidF3aUXCVU3W3VoQFAA"></iframe>

Cet exercice démontre l’opportunité de penser en termes modulaires, ce qui revient souvent en informatique. Ici, on a réalisé qu’un additionneur complet résout un sous-problème bien défini d’une addition générale d’un nombre à _n_
 bits, et qu’une fois qu’on a créé un tel additionneur, il suffit d’en connecter plusieurs les uns derrière les autres de manière structurée pour additionner des nombres plus grands.

## Exercice 2

 Le schéma ci-dessous montre le même additionneur de demi-octets de l’exercice précédent, mais, de plus, la valeur en base 10 de ses 4 bits d’entrée pour `A` 
 et pour `B` est affichée avec un module d’affichage spécial à droite. 
 
 La même chose est faite pour représenter la valeur `S = A + B` (mais seulement sur les quatre premiers bits de `S`). Actuellement, le circuit effectue le calcul 0 + 0 = 0.

Réglez les entrées du circuit de manière à lui faire effectuer les additions suivantes, et vérifiez le résultat. Dans quelles circonstances est-il correct et pourquoi est-il de temps en temps incorrect ? Comment, en regard de ceci, interpréter le bit de sortie `S4`, qui est la retenue de l’additionneur de gauche ?

- 1 + 0
- 3 + 1
- 3 + 3
- 10 + 5
- 14 + 1
- 14 + 2
- 15 + 15

<iframe style="width: 100%; height: 468px; border: 0" src="https://logic.modulo-info.ch/?mode=tryout&data=N4NwXAbANA9gDgFwM5mALxjAtmAHABgF8oBjbOGAOwFNLlUBLS-VBATzmrAHInuoKKANoBGACz4oAVnwBdWACcGtBDyT8GAEzABmKJQCGWLtwCCO7sSYjWHE3wExhAJgnS5i5XTUbtkw8Y8ps6WUEzOtpw8DoJgQjpuMvIwSio+Ydoi+kYmpiKhTDqR9pT8sUJiiR4pXqrc6hlgztmBZvgFlGLF0aWOwiIEUM74Usmp3vW+YCJSLSYAQhZWlFLdvL3lzoPDo55pk43iczzzIcsQazFOcTrbI2O16VrTegEL+csA7Jcb1xV3uxq+wazxEzTeJ3axE0DCQcBYwHYUW4MLhABsDGwyn8pBBZiIdLtntwxABaT6hVFwGyIuw8KkYrF9OK42bOACcRO03FwpJEHygBk0mmoCgRSJMQpFCmxwjEEEkOk+RMoPBEED5uH4MAArqpROyhnJiFLRTSJTxTTLmfEFVAlSqeM4RKTnBZYHq4q4hqMTcLRRFacirbKvXaHfImE6NVttZ6hBz7cbBf6FEUg5LU6HROHlZHVdwdC6dO7dfqEvbfR6EOK6dwy9n5ZIpISHsCpjpoBDuABlKHV811hs2zvN1t7CYg7RK469gVlwMW+t67POO0twHjOpT3S4Wc9s7V9NL4fldVjzePA7PHSG7s9pbVroZninv7K6TjoGTqZue9iSlYTgRc6wZTFs1ZKAxE+DxiTEF1KksYgAHcGAUahhATKD5FEaQcMkCAcL0T4cLBKBcFIvR2VIsQoBEDxRHxEQcOGIYdBYtkKKgeJFXY7iyJEEj+L0ZxnBooYhMY+0xO45p1VIoZmO4yQ1yI+0lINe1CNk2ilRYw1biI3TqO4wkoIYkRDXgljaLEGSEysvj4lssRZFkQggA"></iframe>


## Exercice 3

L’additionneur de demi-octets ci-dessous a été endommagé et ne fonctionne plus correctement. Par exemple, lorsqu’on lui demande d’effectuer le calcul 11 + 1, il livre comme réponse 8.

Déterminez quel composant est défectueux dans ce circuit et comment il faudrait le réparer. Vous pouvez changer les entrées pour vérifier ce qui ne fonctionne pas.

<iframe style="width: 100%; height: 468px; border: 0" src="https://logic.modulo-info.ch/?mode=tryout&data=N4NwXAbANA9gDgFwM5mALxjAtmAHABgF8oBjbOGAOwFNLlUBLS-VBATzmrAHInuoKKANoBGACz4oAVnwBdWACcGtBDyT8GAEzABmKJQCGWLtwCCO-iAMAbMCOJMRrDib4CYwgEwTpcxcro1DW1JQ2MeU09uB0pPZ04eN0EwIR0fGXkYJRUgqC07fSMTUxFLGzsYnXjXSn5koTF0vyyA1W51PO1PQvCzfDLbezzKMWrE2vdhEQIoT3wpTOzA9uC7KR6TACELGKkx3gn6zxm5hf8clc67MQ2eTaiYiH2kjxSdE-nF1tz8kT0wralGIAdmeh1eDQ+ZxaFw6v26ALu-SgVkGxE0DCQcBYwHYCW4GKx1gMbDqEKkEHWfzO+W4YgAtMDolBCXAnLiXDxWcTSZMUhT1p4AJw07TcXD0kRAqAGTSaagKHF4kyy+UKMnCMQQSQ6YE0yg8EQQSW4fgwACuqlEQtmcmIqoV7OVPAd6r5qW1UF1+p4nhE9M8FlglpS3igwHynnWADMsiQuERZPa5Qq4hz8a6NaHPd75ExfcbjmaQ0JhV67TKUwoqumVVWs6Ic3q8wbuDp-TogxarWkvQtiN2lZzuN2G1rJFIdNClm04dodNBEdwAMr9AeWp3D0fuhcTqdfWGrXW3FfS7tp50jy0NzyeyfT76XfLvE-Lh7BhA1y-b+pGvcPw8rh0G0l2XHYP1GWseB-CE9WkfdzmWOcwB8UCxGZVkL2HbkSQbAUoDEYE-FpMR-UaaJiAAdwYBRqGEUsCPkURpCYyQICYvRgSYkRulwbi9CFbibhEPxRCpEQmLmWYdEkwU+KgVIdRkhSeKgEQuJUvRPE8ITZg0sSvR0hTuiNbjZgkhTJFvDivQs60vXY4ybl1SSbXeDjnMEhSpwI0SRBtUjJJuMQjNLALlNSYKxFkJMgA"></iframe>

## Incrémenter i

Additionner 1 à un nombre binaire est une opération très fréquente. Elle est utilisée pour incrémenter le compteur de programme `pc` (program counter), pour pointer à la prochaine instruction.

Complétez le circuit pour incrémenter la variable `i`. Dans beaucoup de langages de programmation, une variable incrémentée est désignée par `i++`.
En Python nous écrivons `i = i + 1`.

D’ailleurs le nom du langage de programmation C++ est une référence à cet opérateur d’incrémentation.

<iframe style="width: 150%; height: 420px; border: 0" src="https://logic.modulo-info.ch/?mode=full&showonly=in,out,in.nibble,out.nibble-display,adder&data=N4NwXAbANA9gDgFwM5mAXygYxgWzjAOwFMDlUBLAgBlQQE84iwByS5qfFAbQFYqoA7FQC6UcgBMWVALQBmdgCNyZACxQQAQwA2LAIz6qzDOPJI4NYPUYsTZrRrrtOYLipX8hoiSxXSB7Ag0cJlYjKFs4XVoGEIj7Rw4Ybjd+WSoRMUlmHghpHgBOAKCQ8gBqUrCNcXEiACcLKxCqmtqnJJdZfP5dLq8CFgAmHmkB-1gAVwQXAYAOKAH84QxmuqjLGJYV1sTuHu7esX7mWWHZMZhJjrnOpagtgejrZi227i6oPb6fAek3dgupq4eFAVBBbltZI8mtU6q9pu9PocfAJfoUJoC+FAeLolhgAO7kWpEbhcfgqURcXRYikDKBgqBcWSCCmdEHkhkLEGLBnYqBnYRLIA"></iframe>


## Décrementer i

Soustraire 1 à un nombre binaire est une opération très fréquente. Elle est utilisée pour décrémenter un compteur de boucle `i`, un pointeur de pile `sp` (stack pointer), ou un pointeur `p` vers les adresses de la mémoire.

Complétez le circuit pour décrémenter la variable `i`. Dans beaucoup de langages de programmation, une variable incrémentée est désignée par `i--`.
En Python nous écrivons `i = i - 1`.

Astuce : pour décrémenter la valeur `i` il suffit d’additionner 1111 qui représente la valeur -1 en format signé.

<iframe style="width: 150%; height: 460px; border: 0" src="https://logic.modulo-info.ch/?mode=full&showonly=in,out,in.nibble,out.nibble-display,adder&data=N4NwXAbANA9gDgFwM5mAXygYxgWzjAOwFMDlUBLAgBlQQE84iwByS5qfFAbQFYqoA7FQC6UcgBMWVALQBmdgCNyZACxQQAQwA2LAIz6qzDOPJI4NYPUYsTZrRrrtOYLipX8hoiSxXSB7Ag0cJlYjKFs4XVoGEIj7Rw4Ybjd+WT4vSWYeCGkeAE4AoJDyaWkwjXFxIgAnCysQiqrqpySXWTz+ACZ3LwIWTp5pTv9YAFcEF06ADihOvOEMRpqoyxiWJebE7l0O2Z6xPuY0uRGYcbaZ9oWoDc7o62YNlu5d7pEDn07pN3YzidceFAVBBrhtZPcGpUas9Jq99pQfAJvgUxv8+FAeLoFhgAO7kapEbhcfgqURcXQYsmdKAgqBcWSCMntIGkulzIHzOmYqCyATCBZAA"></iframe>


## Changer de signe (-i)

Les nombres signés sont représentés avec le format complément à deux. Pour un nombre 4-bits, ceci nous donne une plage de -8 à +7 pour des entiers relatifs, et une plage de 0 à 15 pour des entiers naturels. Nous constatons que la plage signée n’est pas symétrique: le côté négatif compte un nombre en plus.

![Schéma des sept segments](./img/4bits_Integers.svg)


L’opération pour trouver le nombre négatif est: inverser tous les bits (symbolisé par `~`) et additionner 1.
Mathématiquement nous pouvons exprimer cette opération comme:

```
-i = ~i + 1
```

Par exemple, pour obtenir la représentation binaire de -1 nous inversons 0001, ce qui donne 1110 et nous additionnons 1, ce qui donne 1111.

Complétez le circuit pour inverser le signe de la variable `i` et obtenir son négatif `-i`.

<iframe style="width: 150%; height: 480px; border: 0" src="https://logic.modulo-info.ch/?mode=full&showonly=in,out,not,in.nibble,out.nibble-display,adder&data=N4NwXAbANA9gDgFwM5mAXygYxgWzjAOwFMDlUBLAgBlQQE84iwByS5qfFAbQFYqoA7FQC6UcgBMWVALQBmdgCNyZACxQQAQwA2LAIz6qzDOPJI4NYPUYsTZrRrrtOYLipX8hoiSxXSB7Ag0cJlZ2ACcNEwAPMGldKmNTOF1aBhDbOHtHDhhuFQh+WU8xSWYeCGkeAE4AoJDpcnDI8hi4hKgCGAQLKxDOhCdclyr+XQAOEVgw8hIEFiR2SkhdWABXOYgAJgxI8SIwnrSWXf3BvPioTYKvAhZNnmlN-zW5rk2xy6rhHfE9sJTLEdmCcwmcXJsLldJktmLIHkV2DB1i5ZB9ZF8fn9NqlrMDfqcctwDJdrmJbswVJtpG5EcjXDwoPlvlAQbIcSEQWCuLJIaSYSoBNSai8XHwoDxdN8MAB3chhIjcLj8FSiLgrHiqzZQCCq2SCXVVRkqqBvQ0qL4miVQIqqraMza67WSk0qBnVYTfIA"></iframe>

## Soustraction (a-b)

Pour soustraire deux nombres `a-b` il suffit d’additionner le nombre négatif du deuxième (`-b`). Ce nombre négatif peut être obtenu en inversant tous les bits et additionner 1.
Donc `-b = ~b + 1`.

Complétez le circuit pour soustraire `a-b`. Le résultat de 10-3 devrait être 7.

<iframe style="width: 150%; height: 550px; border: 0" src="https://logic.modulo-info.ch/?mode=full&showonly=in,out,not,in.nibble,out.nibble-display,adder&data=N4NwXAbANA9gDgFwM5mAXygYxgWzjAOwFMDlUBLAgBlQQE84iwByS5qfFAbQBYqoAjFSoBdKOQAmLKgFoAzOwBG5MjyggAhgBsWQocwyUBtBk1YF2nML34AmIWMksIcmRAhKVKNZp3NhAgIGUBLkSHA0wPSMLKHhWhp0ljDcgfxCouJSzDwyAOzsBBo4ZhrBcXDGUaaxYXAJSRwp1jx8gnyO2QCsEDJdAJyFxaUyiuV1tiYxzBUNyalCUPaZTsx5vXmDUEUlLGMYBDAIkdFmhwjz1rZd-P0rBGAAHNAwAK4IT3kYGhISRABOJxqzB+f3+ly4cjk6QcsH+5BIH2YFnED2Y1xktgKsHeV0eS36Im+vwBVVOLFBAIhUP40MyMHhiJYKMoLDkXXk2LeH0h+LkhOJYMm1WmlPBTW4NKgfHpjNIzPYrJythkrXY3JaXWlECJUDFcimpRJ4qskOhS1hDIR8uRirRPDyqq2Gq4NygXQERIwAHdyP8iNwuPweGIuAJ3aHbFAdVBIVA8qH+dKQ7HbP1pYTYx6oHIE6n8T1Q3YuqGXPGY1wIGo8nnK1q8o9S9BNqHHnklhWy88RESgA"></iframe>


### Source

https://apprendre.modulo-info.ch/
