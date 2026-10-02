# Étape 0 : Les fondations

Dans cette étape, je pose les fondations du projet en commençant par les bonnes questions. 

## 1. Quels textes garder ?
- à quels critères vérifiables un texte est-il gardé ou rejeté (langue, longueur minimale et maximale, date, doublon, données personnelles, texte traduit automatiquement) ?

## 2. Comment savoir qu'un texte est humain ou généré par une IA ?
- sur quoi repose l'étiquette de chaque classe ?
- Textes IA : générés par moi, donc l'étiquette est connue.
- Textes humains : quels sont le seuil de date et les sources fiables ?

## 3. Quels types de texte allons-nous garder ?
-  quelle part pour chaque domaine (article de presse, blog, forum,email, post Facebook ou LinkedIn, message WhatsApp) ?


## 4. Quelle est la différence entre la date du crawl et la date de publication ?
- laquelle utiliser pour garantir qu'un texte est antérieur à l'IA générative?

## 5. Que perd-on et que garde-t-on à l'extraction ?
- que supprime ou conserve à tort l'extraction du texte principal ?

## 6. Que faire d'une page sans date ?
- la rejeter, estimer sa date, ou la garder à part ?

## 7. Textes IA
-  quels modèles, quels sujets, quels prompts, combien de textes ?
Comment les faire correspondre aux sujets et registres des textes humains ?

## 8. Biais temporel
- comment éviter que le modèle apprenne « ancien contre récent » au lieu de « humain contre IA » ?

## 9. Licences et vie privée
- quelles sources puis-je utiliser, et que faire d'un texte contenant un nom ou un numéro de téléphone ?

## 10. Quantités
- combien de textes par classe et par domaine pour la version 0.1 ?

## 11. Critère de réussite 
- à quoi reconnais-je que le corpus v0.1 est assez bon pour passer à la suite ? 