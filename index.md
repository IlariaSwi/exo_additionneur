---
title: "GYAPI - Exercices additionneur"
permalink: /
layout: default
---

# Additionneur - Exercices

## Queston 1

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


### Source

https://apprendre.modulo-info.ch/
