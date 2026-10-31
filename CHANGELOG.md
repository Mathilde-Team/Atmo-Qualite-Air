# Journal des versions

## [Non publié]

- CI et publication : repli GitHub autorisé, publication manuelle sur un tag
  déjà livré dans main, vérification d’ascendance et archives du tag exact.


- README : la section « Licence » devient « Données et licences » (données Atmo Data sous ODbL 1.0, attribution « Source des données : Atmo France/AASQA », mention complémentaire pour les pollens INTERpollens) (#23).

## [0.1.1] — 22/10/2026

- Workflow de release avec le Python de uv (python3 du runner trop
  ancien) (#4).
- Liens et manifest corrigés après le renommage de l'organisation en
  Mathilde-Team.
- Journal de debug complet (SOCLE §8) : entrée et sortie de chaque
  fonction de l'intégration tracées ; scripts journalisés avec loguru.
- Avis en tête du README : développement arrêté, sources conservées.
- Tests : couverture 100 % lignes et branches, seuil bloquant à 95 % (#13).

## [0.1.0] — 19/10/2026

- Version initiale : indice ATMO du jour et de demain, sous-indices NO₂,
  O₃, PM10, PM2,5 et SO₂, indice pollinique du jour (alerte, taxons,
  concentrations), via l'API Atmo Data d'Atmo France.
- Configuration par compte Atmo Data et code INSEE de commune (ou SIREN
  d'EPCI), prérempli avec Strasbourg (`67482`), avec vérification du
  compte et de la présence d'indices pour le territoire.
- Jeton JWT renouvelé automatiquement ; réauthentification proposée si
  les identifiants sont refusés.
- Pour chaque jour, la diffusion la plus récente est retenue.
