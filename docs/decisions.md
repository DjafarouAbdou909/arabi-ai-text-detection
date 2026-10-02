# Décisions du projet

## 1. Quels textes garder ?
- Seuls les textes en français sont conservés. Les textes traduits sont exclus.
- Longueur minimale : 30 mots. La longueur de chaque texte est enregistrée et les distributions sont comparées entre les classes.
- Sont rejetés : doublons, spam, textes automatiques, textes contenant des
  données personnelles.

## 2. Comment savoir qu'un texte est humain ou généré par une IA ?
- L'étiquette vient de la provenance, jamais du style.
- HUMAN : texte antérieur à 2020 avec source identifiée, ou texte récent fourni par un volontaire qui atteste l'avoir écrit sans IA.
- AI : texte que nous générons nous-mêmes avec modèle et prompt connus.
- Part de textes humains récents : 40 % (environ 60 récents et 90 anciens par
  domaine). Une partie est réservée au test.
- Un échantillon de chaque lot est relu à la main avant validation.

## 3. Types de textes (domaines de la v0.1)
- Posts de réseaux sociaux et articles de blog ou d'actualité.
- Pas de collecte automatique sur Facebook ou LinkedIn. Posts : fournis par des volontaires, avec consentement.
- Les mêmes genres existent dans les deux classes.

## 4. Date du crawl ou date de publication ?
- Date de publication uniquement, enregistrée en métadonnée.

## 5. Extraction
- Contenu principal conservé. Publicités et menus exclus.
- Commentaires exclus (décision provisoire, à retester sur des pages réelles).

## 6. Page sans date
- Exclue de la classe HUMAN. Peut être gardée à part, hors entraînement et test.

## 7. Textes générés par IA
- Cinq familles : Mistral, ChatGPT (OpenAI), Gemini (Google), Claude, Grok.
- Même genre et mêmes sujets que les textes humains. Prompts calibrés pour
  correspondre à la distribution de longueur des textes humains.
- Pour chaque texte : nom exact et version du modèle, prompt, date.

## 8. Biais temporel
- Date enregistrée pour chaque texte. Split temporel prévu.
- Années et dates explicites masquées avant l'entraînement.

## 9. Licences et vie privée
- Aucune donnée personnelle identifiable. Consentement écrit conservé à part,
  stockage privé des textes de volontaires. Licence de chaque source vérifiée.

## 10. Quantités
- 2 domaines, environ 150 textes par domaine et par classe, soit environ 600 textes.

## 11. Critères de réussite (corpus v0.1)
- Au moins 90 % de textes valides sur un échantillon relu de 50 textes,
  avec 0 erreur d'étiquette. Absence de doublons, classes équilibrées.
- Les seuils de performance du modèle seront fixés après les premiers résultats.

## Métadonnées par texte
classe, longueur, domaine, genre, date de publication, source, modèle et version
(si IA), prompt (si IA), licence, consentement, version du filtre