# Médias de Taxi Bourgoin

Ce dépôt public sert à une seule chose : mettre en ligne les médias finis (Reels, images) que Buffer
va chercher pour publier sur Instagram et sur LinkedIn. Une fois publiés, ces médias sont publics de
toute façon.

- Il est rempli par l'atelier réseaux sociaux de Taxi Bourgoin (dépôt privé), avec la commande
  `node atelier.mjs medias envoyer --vraiment`, après un nouveau contrôle de chaque média : rendu en mode
  publication, contrôle réussi, fichier identique au rendu contrôlé, nouvelle mesure de la vidéo ou de
  l'image.
- Il ne contient ni code, ni description, ni photo d'origine.
- Adresse d'un média : `https://resaura.github.io/taxi-bourgoin-medias/m/<empreinte>/<fichier>`.
  L'empreinte vient du contenu du fichier : la même vidéo garde toujours la même adresse.
- `manifeste.json` liste les médias en ligne (empreinte sha256, taille, type, post d'origine, date d'envoi).

Ne rien y déposer à la main : seul l'atelier y écrit (`node atelier.mjs medias auditer` vérifie que le
dépôt ne contient que des médias contrôlés).
