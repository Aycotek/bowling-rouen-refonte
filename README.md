# Bowling de Rouen, refonte indépendante

Site statique en français, conçu pour téléphone et ordinateur. Projet non officiel, sans affiliation ni validation de l'établissement. Le domaine officiel n'est pas modifié.

## Ouvrir le site

La version publiée `index.html` est autonome : styles, scripts et photos optimisées sont intégrés. Télécharger ce fichier puis l’ouvrir dans un navigateur, ou lancer `python3 -m http.server 8080` puis ouvrir http://localhost:8080. Aucun build ni dépendance requis pour utiliser le site. Les liens relatifs sont compatibles avec GitHub Pages, sans domaine personnalisé.

## Fonctionnalités

- Mise en page responsive, navigation mobile avec état accessible et fermeture par Échap.
- Informations clés, activités, tarifs, événements, anniversaire, horaires et accès.
- Téléphone et e-mail directs vers l'établissement. Aucun faux formulaire, réservation, paiement ni disponibilité simulée.
- FAQ native utilisable au clavier. Aucun traceur, cookie applicatif ou collecte de données.
- Photos locales optimisées en WebP et favicon SVG original.

## Sources et droits

Contenus consultés le 23 novembre 2026 :

- https://www.lebowlingderouen.com/
- https://www.lebowlingderouen.com/tarifs
- https://www.lebowlingderouen.com/anniv
- https://www.lebowlingderouen.com/about-4-2
- https://www.lebowlingderouen.com/about-4-3
- https://www.lebowlingderouen.com/about-4-4

Les photographies et la grille tarifaire proviennent du site du Bowling de Rouen. Le commanditaire a confirmé disposer de l'accord du bowling pour leur republication dans cette refonte. Cela ne revendique ni propriété du commanditaire, ni licence libre générale. Sources des photographies :

- https://static.wixstatic.com/media/d0b9e1_e0d0dbc088e24011b89841193d818b39~mv2.jpg
- https://static.wixstatic.com/media/d0b9e1_88e248419ee34b0fa03ef902d40bd014~mv2.jpg
- https://static.wixstatic.com/media/d0b9e1_b6f3e29031c54749847bdcc06582233a~mv2.jpg
- https://static.wixstatic.com/media/d0b9e1_aa8e8fc3a8314497ae63321defc918b8~mv2.png
 Photos recadrées par le design et converties en WebP ; grille tarifaire conservée sans modification de son contenu. Ne pas réutiliser les images hors de ce périmètre sans autorisation des ayants droit.

Aucune licence générale n'est accordée par ce dépôt. Les marques et contenus de tiers conservent leurs droits.

## Incertitudes du site source

- Anniversaire : la page dédiée indique 14 ans maximum, la page événements 16 ans. Les deux indiquent 14 € par enfant. La refonte conserve l'avertissement au lieu de trancher.
- Dimanche : accueil et plusieurs pages indiquent 14h30, la page carte indique 14h. La refonte affiche 14h30 avec une note explicite.
- Des événements d'avril sans année ne sont pas présentés comme à venir.
- Les prix restent ceux de la source à la date du relevé. La grille originale peut être agrandie ; les conditions et disponibilités sont à confirmer auprès du bowling.

## Tests réalisés

Contrôles à 320, 390, 768 et 1440 px : pas de débordement horizontal, images chargées, ancres existantes et aucune erreur JavaScript. Menu mobile testé par clic et fermeture Échap. FAQ et grille tarifaire testées. Captures ordinateur et mobile inspectées. La version autonome relue depuis GitHub a été rendue à 390 et 1440 px avec toutes les images présentes. Les photos sont compressées pour cette version autonome.

## Audit et choix techniques

Lors du contrôle, le site d'origine affichait un écran orange vide avec un document mesuré à environ 16,8 millions de pixels de hauteur. La refonte utilise un flux CSS normal (grid/flex), sans positions absolues pour le contenu, sans dimensions géantes, sans lecteur vidéo ou moteur de mise en page lourd. Les images ont des dimensions déclarées pour limiter les déplacements de contenu.

Aucun secret, clé API, service tiers de formulaire ou dépendance d'exécution. Les liens externes dans un nouvel onglet ont `noopener`. Les numéros et adresses viennent de la source. Pas de prétention à une certification juridique ou d'accessibilité.

## Maintenance et retour arrière

Le fichier index.html contient le contenu, les styles et le script. Modifier une copie, tester sur téléphone et ordinateur avant publication. Préserver les crédits et vérifier prix/horaires auprès de la source avant usage commercial. Pour revenir en arrière, restaurer le commit précédent. Ne pas connecter le domaine officiel sans autorisation distincte.
