<MenuSchema />

## arrete-circulation-marchandises

Arrêtés permanents de circulation pour le transport de marchandises

Spécification du fichier d'échange relatif aux arrêtés permanents de circulation pour le transport de marchandises gérés par les collectivités.

- Schéma créé le : 04/30/21
- Site web : https://github.com/CEREMA/schema-arrete-circulation
- Version : 0.7.0
- Valeurs manquantes : `""`, `"NA"`, `"NaN"`, `"N/A"`
- Clé primaire : `ID`

### Modèle de données


##### Liste des propriétés

| Propriété | Type | Obligatoire |
| -- | -- | -- |
| [ID](#identifiant-de-l'entite-propriete-id) | chaîne de caractères  | Oui |
| [COLL_NOM](#nom-de-la-collectivite-a-l'origine-de-l'arrete-propriete-coll-nom) | chaîne de caractères  | Oui |
| [COLL_INSEE](#code-insee-propriete-coll-insee) | chaîne de caractères  | Oui |
| [ARR_DATE](#date-de-l'arrete-propriete-arr-date) | date (format `%Y-%m-%d`) | Oui |
| [ARR_REF](#reference-de-l'arrete-propriete-arr-ref) | chaîne de caractères  | Oui |
| [ARR_OBJET](#objet-de-l'arrete-propriete-arr-objet) | chaîne de caractères  | Oui |
| [ARR_CONSIDERANT](#considerant-de-l'arrete-propriete-arr-considerant) | chaîne de caractères  | Non |
| [ARR_URL](#adresse-internet-de-l'arrete-propriete-arr-url) | chaîne de caractères (format `uri`) | Non |
| [REGL_ARTICLE](#article-du-reglement-propriete-regl-article) | chaîne de caractères  | Non |
| [REGL_SOUS_ARTICLE](#sous-article-du-reglement-propriete-regl-sous-article) | chaîne de caractères  | Non |
| [REGL_MODALITE](#modalite-du-reglement-propriete-regl-modalite) | chaîne de caractères  | Oui |
| [VEH_TYPES](#types-de-vehicules-propriete-veh-types) | chaîne de caractères  | Non |
| [VEH_TONNAGE](#tonnage-ou-poids-total-autorise-en-charge-propriete-veh-tonnage) | nombre réel  | Non |
| [VEH_LONG](#longueur-du-vehicule-propriete-veh-long) | nombre réel  | Non |
| [VEH_LARG](#largeur-du-vehicule-propriete-veh-larg) | nombre réel  | Non |
| [VEH_HAUT](#hauteur-du-vehicule-propriete-veh-haut) | nombre réel  | Non |
| [VEH_USAGES](#types-d'usage-propriete-veh-usages) | chaîne de caractères  | Non |
| [VEH_MOTORS](#types-de-motorisation-propriete-veh-motors) | chaîne de caractères  | Non |
| [VEH_CQAS](#vignettes-crit'air-propriete-veh-cqas) | chaîne de caractères  | Non |
| [PERIODE_DEBUT](#date-d'entree-en-vigueur-des-restrictions-propriete-periode-debut) | date (format `%Y-%m-%d`) | Non |
| [PERIODE_JH](#jours-et-heures-de-circulation-propriete-periode-jh) | chaîne de caractères  | Non |
| [EMPRISE_DESIGNATION](#nom-de-la-voie-propriete-emprise-designation) | chaîne de caractères  | Oui |
| [EMPRISE_DEBUT](#debut-de-la-section-(libelle)---propriété-emprise_debut) | chaîne de caractères  | Non |
| [GEOM_DEBUT](#debut-de-la-section-(coordonnees)---propriété-geom_debut) | point géographique  | Non |
| [EMPRISE_FIN](#fin-de-la-section-(libelle)---propriété-emprise_fin) | chaîne de caractères  | Non |
| [GEOM_FIN](#fin-de-la-section-(coordonnees)---propriété-geom_fin) | point géographique  | Non |
| [EMPRISE_SENS](#direction-ou-sens-de-circulation-propriete-emprise-sens) | chaîne de caractères  | Non |
| [INTERV_DUREE](#duree-maximale-d'intervention-propriete-interv-duree) | heure  | Non |
| [INTERV_HMAX](#heure-maximale-d'intervention-propriete-interv-hmax) | heure  | Non |
| [GEOM_WKT](#geometrie-au-format-wkt-propriete-geom-wkt) | chaîne de caractères  | Non |
| [GEOM_SOURCE](#source-de-la-geometrie-propriete-geom-source) | chaîne de caractères  | Non |

#### Identifiant de l'entité - Propriété `ID`

> *Description : Il s'agit de l'identifiant, unique, de la ligne du tableau.. [Vous pouvez créer des identifiants grâce à l'application Heidi d'Etalab](https://heidi.app.etalab.studio/).<br/>Ex : 133-3*
- Valeur obligatoire
- Type : chaîne de caractères

#### Nom de la collectivité à l'origine de l'arrêté - Propriété `COLL_NOM`

> *Description : Nom de la collectivité.<br/>Ex : Commune d'Aix-en-Provence*
- Valeur obligatoire
- Type : chaîne de caractères

#### Code INSEE - Propriété `COLL_INSEE`

> *Description : Code INSEE de la commune sur laquelle s'applique l'arrêté<br/>Ex : 13090*
- Valeur obligatoire
- Type : chaîne de caractères
- Entre 5 et 5 caractères
- Motif : `^([013-9]\d|2[AB1-9])\d{3}$`

#### Date de l'arrêté - Propriété `ARR_DATE`

> *Description : Date de création ou de mise à jour de l'arrêté, au format ISO 8601 AAAA-MM-DD. Mettre `NC` si pas d'indication dans l'arrêté<br/>Ex : 2021-04-30*
- Valeur obligatoire
- Type : date (format `%Y-%m-%d`)

#### Référence de l'arrêté - Propriété `ARR_REF`

> *Description : Référence ou numéro de l'arrêté auquel se réfère la règlementation. Si l'arrêté a été mis à jour, la référence doit être celle de l'arrêté mis à jour et non celle de l'arrêté originel. Si l'arrêté ne possède pas de référence, mettre la valeur `NC`<br/>Ex : AP-13090-12*
- Valeur obligatoire
- Type : chaîne de caractères

#### Objet de l'arrêté - Propriété `ARR_OBJET`

> *Description : Objet ou titre de l'arrêté. Mettre `NC` si l'arrêté ne comprend pas d'objet.<br/>Ex : Arrêté règlementant la circulation dans le quartier Mazarin et du palais de Justice*
- Valeur obligatoire
- Type : chaîne de caractères

#### Considérant de l'arrêté - Propriété `ARR_CONSIDERANT`

> *Description : Considérant est le justificatif de la mise en place de la règlementation. S'il y a plusieurs considérations, les séparer par le caractère '|'<br/>Ex : Considérant la dangerosité que représente le trafic des PL aux abords des groupes scolaires*
- Valeur optionnelle
- Type : chaîne de caractères

#### Adresse internet de l'arrêté - Propriété `ARR_URL`

> *Description : Adresse internet par laquelle accéder à l'arrêté, et donc au règlement.<br/>Ex : https://carte.st-paul-les-dax.fr/wp-content/uploads/2020/06/AM-10248.pdf*
- Valeur optionnelle
- Type : chaîne de caractères (format `uri`)

#### Article du règlement - Propriété `REGL_ARTICLE`

> *Description : N° de l'article associé au règlement lorsqu'il existe<br/>Ex : 4*
- Valeur optionnelle
- Type : chaîne de caractères

#### Sous-article du règlement - Propriété `REGL_SOUS_ARTICLE`

> *Description : Un article peut se décomposer en plusieurs sous-articles, contenant chacun une règlementation particulière. Ces sous-articles ont des numérotations.<br/>Ex : 4 bis*
- Valeur optionnelle
- Type : chaîne de caractères

#### Modalité du règlement - Propriété `REGL_MODALITE`

> *Description : Indique si l'arrêté interdit ou autorise<br/>Ex : Autorise*
- Valeur obligatoire
- Type : chaîne de caractères
- Valeurs autorisées : 
    - Autorise
    - Interdit

#### Types de véhicules - Propriété `VEH_TYPES`

> *Description : Types de véhicules. S'il y a plusieurs types, les séparer les valeurs par le caractère '|'. Les valeurs possibles sont : 'Poids lourds', 'Véhicules utilitaires légers', 'Vélo-cargos' et 'Tous véhicules'.<br/>Ex : Poids lourds|Véhicules utilitaires légers*
- Valeur optionnelle
- Type : chaîne de caractères
- Motif : `(?:(?:^|\|)(Poids lourds|Véhicules utilitaires légers|Vélo-cargos|Tous véhicules))+$`

#### Tonnage ou poids total autorisé en charge - Propriété `VEH_TONNAGE`

> *Description : Tonnage ou poids total autorisé en charge, exprimé en tonnes.<br/>Ex : 7.5*
- Valeur optionnelle
- Type : nombre réel
- Valeur entre 0 et 45

#### Longueur du véhicule - Propriété `VEH_LONG`

> *Description : Longueur maximale exprimée en mètres.<br/>Ex : 6.5*
- Valeur optionnelle
- Type : nombre réel
- Valeur entre 0 et 30

#### Largeur du véhicule - Propriété `VEH_LARG`

> *Description : Longueur maximale exprimée en mètres.<br/>Ex : 3.5*
- Valeur optionnelle
- Type : nombre réel
- Valeur entre 0 et 6

#### Hauteur du véhicule - Propriété `VEH_HAUT`

> *Description : Longueur maximale exprimée en mètres.<br/>Ex : 2.5*
- Valeur optionnelle
- Type : nombre réel
- Valeur entre 0 et 6

#### Types d'usage - Propriété `VEH_USAGES`

> *Description : Types d'usage de véhicule. S'il y a plusieurs usages, séparer les valeurs par le caractère '|'<br/>Ex : Bennes à ordures ménagères|Véhicules de police*
- Valeur optionnelle
- Type : chaîne de caractères

#### Types de motorisation - Propriété `VEH_MOTORS`

> *Description : Types de motorisation. S'il y a plusieurs motorisations, les séparer par le caractère '|'. Les valeurs possibles sont : Electrique, Gaz Naturel pour Véhicules et Hydrogène.<br/>Ex : Électrique|Hydrogène*
- Valeur optionnelle
- Type : chaîne de caractères
- Motif : `(?:(?:^|\|)(Electrique|Gaz Naturel pour Véhicules|Hydrogène))+$`

#### Vignettes crit'air - Propriété `VEH_CQAS`

> *Description : Vignettes crit'air. Voir la [classification des vignettes Crit'Air](https://www.certificat-air.gouv.fr/docs/tableaux_classement.pdf) sur le site [certificat-air.gouv.fr](https://www.certificat-air.gouv.fr). Séparer les étiquettes CQA par le caractère '|'<br/>Ex : 1|2|3*
- Valeur optionnelle
- Type : chaîne de caractères
- Motif : `(?:(?:^|\|)(100% électrique et Véhicules à hydrogène|1|2|3|4|5|Véhicule non classé))+$`

#### Date d'entrée en vigueur des restrictions - Propriété `PERIODE_DEBUT`

> *Description : Date d'entrée en vigueur des restrictions (en particulier pour les Zones à Faible Émission), au format ISO 8601 AAAA-MM-DD.<br/>Ex : 2021-04-30*
- Valeur optionnelle
- Type : date (format `%Y-%m-%d`)

#### Jours et heures de circulation - Propriété `PERIODE_JH`

> *Description : Jours et heures de circulation autorisés pour la circulation exprimés selon le format OpeningHours d'OpenStreetMap ([https://wiki.openstreetmap.org/wiki/Key:opening_hours](https://wiki.openstreetmap.org/wiki/Key:opening_hours)). Ce format permet d'indiquer les week-ends (we), les jours fériés (PH) et les vacances scolaires (SH). Par exemple `Mo-Fr 09:00-17:00; PH 10:00-12:00; PH Su off` signifie : 'Du lundi au vendredi de 9h à 17h sauf les jours fériés où l'ouverture est de 10h à 12h, à l'exception des jours fériés tombant un dimanche'. `24/7` indique `Tous les jours`. [Utiliser groom-groom pour récupérer les jours et heures de circulation](https://cerema-med.shinyapps.io/groom-groom?action=opening_hours)<br/>Ex : Mo-Fr 08:00-12:00,13:00-17:30; Sa 08:00-12:00; PH off*
- Valeur optionnelle
- Type : chaîne de caractères

#### Nom de la voie - Propriété `EMPRISE_DESIGNATION`

> *Description : Nom de la voie, ou de la zone associée à la section règlementée. La zone peut être une aire piétonne, un quartier, une zone ZFE ([voir le schéma des ZFE](https://schema.data.gouv.fr/etalab/schema-zfe/latest.html))<br/>Ex : Avenue Philippe Solari, Commune d'Aix-en-Provence, Quartier Mazarin, 200046977-ZFE-001*
- Valeur obligatoire
- Type : chaîne de caractères
- Motif : `^[a-zA-Z0-9\-\–\'\’\s\d\u00C0-\u00FF\(\)]+$`

#### Début de la section (libellé) - Propriété `EMPRISE_DEBUT`

> *Description : Indication textuelle de l'endroit à partir duquel la règlementation s'applique, telle qu'écrite dans l'arrêté. Pour indiquer les coordonnées GPS, se référer au champ `GEOM_DEBUT`.<br/>Ex : 22 avenue Philippe Solari, Croisement de l'avenue Philippe Solari avec la rue Gaston de Saporta*
- Valeur optionnelle
- Type : chaîne de caractères

#### Début de la section (coordonnées) - Propriété `GEOM_DEBUT`

> *Description : Coordonnées GPS du début de la section. Se réfère à `EMPRISE_DEBUT`. S'écrit sous la forme 'long,lat' (5 ou 6 décimales sont conseillées).<br/>Ex : 5.42101,43.53591*
- Valeur optionnelle
- Type : point géographique

#### Fin de la section (libellé) - Propriété `EMPRISE_FIN`

> *Description : Indication textuelle de l'endroit au bout duquel la règlementation s'applique, telle qu'écrite dans l'arrêté. Pour indiquer les coordonnées GPS, se référer au champ `GEOM_FIN`.<br/>Ex : 34 bis avenue Philippe Solari, Intersection de l'avenue Philippe Solari avec le boulevard des Charmettes*
- Valeur optionnelle
- Type : chaîne de caractères

#### Fin de la section (coordonnées) - Propriété `GEOM_FIN`

> *Description : Coordonnées GPS de la fin de la section. Se réfère à `EMPRISE_DEBUT`. S'écrit sous la forme 'long,lat' (5 ou 6 décimales sont conseillées).<br/>Ex : 5.42101,43.53591*
- Valeur optionnelle
- Type : point géographique

#### Direction ou sens de circulation - Propriété `EMPRISE_SENS`

> *Description : Direction ou sens de circulation associé à la règlementation. Pair : concerne la circulation le long des adresses à chiffre pair. `Nord` signifie vers le Nord, soit "vers le haut".<br/>Ex : Deux sens, Impair, Nord*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - Pair
    - Impair
    - Nord
    - Sud
    - Est
    - Ouest
    - Deux sens

#### Durée maximale d'intervention - Propriété `INTERV_DUREE`

> *Description : Durée maximale d'intervention (au niveau d'une aire piétonne, par exemple). L'entrée et la sortie dans une zone peuvent être horodatées à la délivrance d'un ticket lors de la traversée d'une borne de passage.<br/>Ex : 03:00:00*
- Valeur optionnelle
- Type : heure

#### Heure maximale d'intervention - Propriété `INTERV_HMAX`

> *Description : Heure max à partir de laquelle les véhicules doivent quitter l'aire piétonne.<br/>Ex : 22:00:00*
- Valeur optionnelle
- Type : heure

#### Géométrie au format WKT - Propriété `GEOM_WKT`

> *Description : Géométrie de la rue (ligne), ou de l'emprise (polygone) exprimée au format [WKT (Well Know Text](https://fr.wikipedia.org/wiki/Well-known_text) sous le système de projection WGS84 (EPSG:4326)<br/>Ex : LineString(5.39340184 45.56538751, 5.41017215 45.56722934, 5.42510063 45.5679079)*
- Valeur optionnelle
- Type : chaîne de caractères

#### Source de la géométrie - Propriété `GEOM_SOURCE`

> *Description : Source de la donnée depuis laquelle la donnée a été extraite (OpenStreetMap, IGN,...).<br/>Ex : BDTOPO IGN 2021*
- Valeur optionnelle
- Type : chaîne de caractères
