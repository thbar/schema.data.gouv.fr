<MenuSchema />

## acceslibre

Schéma des données d'accessibilité des ERPs

Spécification du fichier d'échange relatif aux données d'accessibilité des Établissements Recevant du Public (ERP).

- Schéma créé le : 03/10/21
- Site web : https://github.com/MTES-MCT/acceslibre-schema
- Version : 0.0.14
- Clé primaire : `id`

### Modèle de données


##### Liste des propriétés

| Propriété | Type | Obligatoire |
| -- | -- | -- |
| [id](#propriete-id) | chaîne de caractères  | Oui |
| [name](#propriete-name) | chaîne de caractères  | Oui |
| [postal_code](#propriete-postal-code) | chaîne de caractères  | Oui |
| [commune](#propriete-commune) | chaîne de caractères  | Oui |
| [numero](#propriete-numero) | chaîne de caractères  | Non |
| [voie](#propriete-voie) | chaîne de caractères  | Non |
| [lieu_dit](#propriete-lieu-dit) | chaîne de caractères  | Non |
| [code_insee](#propriete-code-insee) | chaîne de caractères  | Non |
| [siret](#propriete-siret) | chaîne de caractères  | None |
| [contact_url](#propriete-contact-url) | chaîne de caractères (format `uri`) | Non |
| [site_internet](#propriete-site-internet) | chaîne de caractères (format `uri`) | Non |
| [longitude](#propriete-longitude) | nombre réel  | Non |
| [latitude](#propriete-latitude) | nombre réel  | Non |
| [activite](#activite-propriete-activite) | chaîne de caractères  | None |
| [transport_station_presence](#proximite-d'un-arret-de-transport-en-commun-propriete-transport-station-presence) | booléen  | Non |
| [stationnement_presence](#stationnement-dans-l'etablissement-propriete-stationnement-presence) | booléen  | Non |
| [stationnement_pmr](#stationnements-adaptes-dans-l'etablissement-propriete-stationnement-pmr) | booléen  | Non |
| [stationnement_ext_presence](#stationnement-a-proximite-de-l'etablissement-propriete-stationnement-ext-presence) | booléen  | Non |
| [stationnement_ext_pmr](#stationnements-adaptes-a-proximite-de-l'etablissement-propriete-stationnement-ext-pmr) | booléen  | Non |
| [cheminement_ext_presence](#chemin-exterieur-propriete-cheminement-ext-presence) | booléen  | Non |
| [cheminement_ext_terrain_stable](#revetement-exterieur-propriete-cheminement-ext-terrain-stable) | booléen  | Non |
| [cheminement_ext_plain_pied](#chemin-exterieur-de-plain-pied-propriete-cheminement-ext-plain-pied) | booléen  | Non |
| [cheminement_ext_ascenseur](#ascenseur/elevateur-propriete-cheminement-ext-ascenseur) | booléen  | Non |
| [cheminement_ext_nombre_marches](#nombre-de-marches-propriete-cheminement-ext-nombre-marches) | nombre entier  | Non |
| [cheminement_ext_reperage_marches](#marches-ou-escalier-securise(es)---propriété-cheminement_ext_reperage_marches) | booléen  | Non |
| [cheminement_ext_sens_marches](#sens-de-circulation-de-l'escalier-propriete-cheminement-ext-sens-marches) | chaîne de caractères  | None |
| [cheminement_ext_main_courante](#main-courante-propriete-cheminement-ext-main-courante) | booléen  | Non |
| [cheminement_ext_rampe](#rampe-propriete-cheminement-ext-rampe) | chaîne de caractères  | None |
| [cheminement_ext_pente_presence](#pente-propriete-cheminement-ext-pente-presence) | booléen  | Non |
| [cheminement_ext_pente_degre_difficulte](#degre-de-difficulte-de-la-pente-propriete-cheminement-ext-pente-degre-difficulte) | chaîne de caractères  | None |
| [cheminement_ext_pente_longueur](#longueur-de-la-pente-propriete-cheminement-ext-pente-longueur) | chaîne de caractères  | None |
| [cheminement_ext_devers](#devers-propriete-cheminement-ext-devers) | chaîne de caractères  | None |
| [cheminement_ext_bande_guidage](#bande-de-guidage-propriete-cheminement-ext-bande-guidage) | booléen  | Non |
| [cheminement_ext_retrecissement](#retrecissement-du-chemin-propriete-cheminement-ext-retrecissement) | booléen  | Non |
| [entree_reperage](#entree-facilement-reperable-propriete-entree-reperage) | booléen  | Non |
| [entree_vitree](#entree-vitree-propriete-entree-vitree) | booléen  | Non |
| [entree_vitree_vitrophanie](#reperage-de-la-vitre-propriete-entree-vitree-vitrophanie) | booléen  | Non |
| [entree_plain_pied](#entree-de-plain-pied-propriete-entree-plain-pied) | booléen  | Non |
| [entree_ascenseur](#ascenseur/elevateur-propriete-entree-ascenseur) | booléen  | Non |
| [entree_marches](#nombre-de-marches-propriete-entree-marches) | nombre entier  | Non |
| [entree_marches_reperage](#reperage-des-marches-propriete-entree-marches-reperage) | booléen  | Non |
| [entree_marches_main_courante](#main-courante-propriete-entree-marches-main-courante) | booléen  | Non |
| [entree_marches_rampe](#rampe-propriete-entree-marches-rampe) | chaîne de caractères  | None |
| [entree_marches_sens](#sens-de-circulation-de-l'escalier-propriete-entree-marches-sens) | chaîne de caractères  | None |
| [entree_dispositif_appel](#dispositif-d'appel-a-l'entree-propriete-entree-dispositif-appel) | booléen  | Non |
| [entree_dispositif_appel_type](#type-de-dispositif-d'appel-a-l'entree-propriete-entree-dispositif-appel-type) | liste  | Non |
| [entree_balise_sonore](#balise-sonore-a-l'entree-propriete-entree-balise-sonore) | booléen  | Non |
| [entree_aide_humaine](#aide-humaine-propriete-entree-aide-humaine) | booléen  | Non |
| [entree_largeur_mini](#largeur-de-la-porte-propriete-entree-largeur-mini) | nombre entier  | Non |
| [entree_pmr](#entree-specifique-pmr-propriete-entree-pmr) | booléen  | Non |
| [entree_porte_presence](#y-a-t-il-une-porte ?-propriete-entree-porte-presence) | booléen  | Non |
| [entree_porte_manoeuvre](#manoeuvre-de-la-porte-propriete-entree-porte-manoeuvre) | chaîne de caractères  | None |
| [entree_porte_type](#type-de-porte-propriete-entree-porte-type) | chaîne de caractères  | None |
| [accueil_visibilite](#visibilite-de-la-zone-d'accueil-propriete-accueil-visibilite) | booléen  | Non |
| [accueil_personnels](#personnel-d'accueil-propriete-accueil-personnels) | chaîne de caractères  | None |
| [accueil_audiodescription_presence](#audiodescription-propriete-accueil-audiodescription-presence) | booléen  | Non |
| [accueil_audiodescription](#liste-des-equipements-pour-l'audiodescription-propriete-accueil-audiodescription) | liste  | Non |
| [accueil_equipements_malentendants_presence](#presence-d'equipements-d'aide-a-l'audition-et-a-la-communication-propriete-accueil-equipements-malentendants-presence) | booléen  | Non |
| [accueil_equipements_malentendants](#liste-des-equipements-d'aide-a-l'audition-et-a-la-communication-propriete-accueil-equipements-malentendants) | liste  | Non |
| [accueil_cheminement_plain_pied](#chemin-entre-l'entree-principale-du-batiment-et-l'accueil-de-l'etablissement-propriete-accueil-cheminement-plain-pied) | booléen  | Non |
| [accueil_cheminement_ascenseur](#ascenseur/elevateur-propriete-accueil-cheminement-ascenseur) | booléen  | Non |
| [accueil_cheminement_nombre_marches](#nombre-de-marches-propriete-accueil-cheminement-nombre-marches) | nombre entier  | Non |
| [accueil_cheminement_reperage_marches](#reperage-des-marches-ou-de-l'escalier-propriete-accueil-cheminement-reperage-marches) | booléen  | Non |
| [accueil_cheminement_main_courante](#main-courante-propriete-accueil-cheminement-main-courante) | booléen  | Non |
| [accueil_cheminement_rampe](#rampe-propriete-accueil-cheminement-rampe) | chaîne de caractères  | None |
| [accueil_cheminement_sens_marches](#sens-de-circulation-de-l'escalier-propriete-accueil-cheminement-sens-marches) | chaîne de caractères  | None |
| [accueil_chambre_nombre_accessibles](#nombre-de-chambres-accessibles-a-une-personne-en-fauteuil-roulant-propriete-accueil-chambre-nombre-accessibles) | nombre entier  | Non |
| [accueil_chambre_douche_plain_pied](#douche-accessible-propriete-accueil-chambre-douche-plain-pied) | booléen  | Non |
| [accueil_chambre_douche_siege](#siege-de-douche-propriete-accueil-chambre-douche-siege) | booléen  | Non |
| [accueil_chambre_douche_barre_appui](#douche-securisee-propriete-accueil-chambre-douche-barre-appui) | booléen  | Non |
| [accueil_chambre_sanitaires_barre_appui](#toilette-securise-propriete-accueil-chambre-sanitaires-barre-appui) | booléen  | Non |
| [accueil_chambre_sanitaires_espace_usage](#toilette-accessible-propriete-accueil-chambre-sanitaires-espace-usage) | booléen  | Non |
| [accueil_chambre_numero_visible](#visibilite-des-numeros-de-chambres-propriete-accueil-chambre-numero-visible) | booléen  | Non |
| [accueil_chambre_equipement_alerte](#equipement-d'alerte-adapte-propriete-accueil-chambre-equipement-alerte) | booléen  | Non |
| [accueil_chambre_accompagnement](#accompagnement-specifique-propriete-accueil-chambre-accompagnement) | booléen  | Non |
| [accueil_retrecissement](#retrecissement-du-chemin-propriete-accueil-retrecissement) | booléen  | Non |
| [sanitaires_presence](#sanitaires-propriete-sanitaires-presence) | booléen  | Non |
| [sanitaires_adaptes](#sanitaires-adaptes-propriete-sanitaires-adaptes) | booléen  | Non |
| [labels](#marques-ou-labels-propriete-labels) | liste  | Non |
| [labels_familles_handicap](#famille(s)-de-handicap-concernées(s)---propriété-labels_familles_handicap) | liste  | Non |
| [registre_url](#registre-propriete-registre-url) | chaîne de caractères (format `uri`) | Non |
| [conformite](#conformite-propriete-conformite) | booléen  | Non |

#### Propriété `id`

> *Description : Identifiant unique<br/>Ex : 123e4567-e89b-12d3-a456-426614174000*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `name`

> *Description : Nom de l'établissement<br/>Ex : Mairie du 3e*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `postal_code`

> *Description : Code postal<br/>Ex : 75017*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `commune`

> *Description : Nom de la commune<br/>Ex : Paris 17*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `numero`

> *Description : Numero de la rue<br/>Ex : 15*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `voie`

> *Description : Nom de la rue/voie<br/>Ex : Rue Paul Chenavard*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `lieu_dit`

> *Description : Lieu-dit<br/>Ex : Le petit Marché*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `code_insee`

> *Description : Code INSEE<br/>Ex : 17877*
- Valeur obligatoire
- Type : chaîne de caractères

#### Propriété `siret`

> *Description : Le numero SIRET de l'ERP issue de la base SIRENE des entreprises. Vous pouvez récupérer cet identifiant sur le site annuaire-entreprises.data.gouv.fr.<br/>Ex : 13002526564591*
- Valeur optionnelle
- Type : chaîne de caractères
- Motif : `^\d{14}$`

#### Propriété `contact_url`

> *Description : Lien vers un moyen de contact (chatbot, formulaire, ...)<br/>Ex : https://site.com/contact*
- Valeur optionnelle
- Type : chaîne de caractères (format `uri`)

#### Propriété `site_internet`

> *Description : Site internet de l'établissement<br/>Ex : https://site.com/*
- Valeur optionnelle
- Type : chaîne de caractères (format `uri`)

#### Propriété `longitude`

> *Description : Coordonnées GPS: longitude<br/>Ex : 2.352222*
- Valeur optionnelle
- Type : nombre réel

#### Propriété `latitude`

> *Description : Coordonnées GPS: latitude<br/>Ex : 48.856613*
- Valeur optionnelle
- Type : nombre réel

#### Activité - Propriété `activite`

> *Description : Domaine d'activité de l'ERP<br/>Ex : Mairie*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - Accessoires
    - Accompagnement personnes agees
    - Accrobranche
    - Achat or
    - Administration publique
    - Aéroport
    - Afpa
    - Agence départementale d'information sur le logement
    - Agence de publicité
    - Agence de travail temporaire
    - Agence de voyage
    - Agence immobilière
    - Agence matrimoniale
    - Agence postale
    - Aide à la personne
    - Aide sociale à l'enfance : action éducative
    - Ambulances
    - Aménagement maison : cuisine salle de bain salon
    - Anesthésie
    - Animalerie
    - Antiquaire
    - Apiculteur
    - Aquarium
    - Architecte
    - Arène
    - Armurerie coutellerie
    - Art
    - Artisanat
    - Arts de la table
    - Association
    - Association aide aux victimes
    - Association de gestion du fonds pour l'insertion professionnelle des personnes handicapées
    - Assurance
    - Athlétisme
    - Audio prothésiste
    - Auditorium et salle de conférence
    - Auto école
    - Autre
    - Autres établissements pour adultes et familles en difficulté
    - Avocat
    - Banques, caisses d'épargne
    - Barbier
    - Bar tabac
    - Bâtiment d'accueil
    - Bazar
    - Bibliothèque médiathèque
    - Bien-être
    - Bijouterie joaillerie
    - Biscuiterie
    - Blanchisserie teinturerie
    - Boucherie / commerce de viande
    - Boulangerie
    - Boulangerie Pâtisserie
    - Boulodrome
    - Boutique de mariage
    - Bowling
    - Bricolage, matériaux, travaux
    - Brocante
    - Brûlerie
    - Bureau de douane
    - Bureau de poste
    - Café, bar, brasserie
    - Cafés et thés
    - Caisse d'allocations familiales (caf)
    - Camping caravaning
    - Cantine
    - Cardiologie
    - Carrosserie
    - Casino
    - Caviste / commerce de détail de boissons
    - Centrale nucléaire
    - Centre commercial
    - Centre culturel
    - Centre de gestion de la fonction publique territoriale
    - Centre de loisirs
    - Centre de protection maternelle et infantile (pmi)
    - Centre de ressources et d'information
    - Centre de vacances
    - Centre de vaccination
    - Centre d'examen
    - Centre d’information et d’orientation
    - Centre d'information sur les droits des femmes et des familles
    - Centre équestre
    - Centre médical
    - Centre national de la fonction publique territoriale
    - Centre religieux
    - Centre social
    - Chambre agriculture
    - Chambre de commerce et d'industrie
    - Chambre metier
    - Chambres d'hôtes, gîte, pension
    - Chapeaux et couvre-chefs
    - Charcuterie
    - Château
    - Chaussures
    - Chenil, fourrière
    - Chirurgie
    - Chirurgien dentiste
    - Chocolatier
    - Cigarette électronique
    - Cimetière
    - Cinéma
    - Circuit sportif deux roues / voiture
    - Clinique
    - Coiffure
    - Collectivité territoriale
    - Collège
    - Commerce
    - Commerce automobile
    - Commerce bio
    - Commissariat de Police
    - Commission conciliation
    - Communauté de communes
    - Comptable expert-comptable
    - Concessionnaire automobile
    - Confiserie
    - Conservatoire et école de musique
    - Construction de maisons, immeubles
    - Contrôle technique auto
    - Coopérative agricole
    - Cordonnerie serrurerie
    - Courtier
    - Coworking
    - Crèche
    - Crèmerie Fromagerie
    - Cure thermale
    - Cycle vente et entretien
    - Cyclisme
    - Déchetterie
    - Décoration Design
    - Déménageur
    - Dermatologie vénéréologie
    - Direction départementale de la protection des populations
    - Direction départementale de l'emploi, du travail, des solidarités et de la protection des populations
    - Discothèque
    - Disquaire
    - Distribution spécialisée / commerce de gros
    - Droguerie
    - Ecole de danse
    - École élémentaire
    - École maternelle
    - École primaire (regroupement maternelle et élémentaire)
    - EHPAD
    - Électricien
    - Électroménager et matériel audio-vidéo
    - Emploi, formation
    - Encadreur enlumineur
    - Endocrinologue
    - Épicerie
    - Epicerie fine
    - Équipements du foyer
    - Equipement sportif
    - Ergothérapeute
    - Espace collaboratif
    - Espace numérique
    - Espace vert et naturel
    - Etablissement de prévention
    - Établissement de santé
    - Établissement militaire
    - Etablissement pénitentiaire
    - Fédération départementale pour la pêche et la protection du milieu aquatique
    - Fleuriste
    - Friperie
    - Fruits et légumes
    - Galerie d'art
    - Garage automobile
    - Garderie
    - Gare avec desserte train à grande vitesse (TAGV)
    - Gare routière
    - Gare sans desserte train à grande vitesse (TAGV)
    - Gastro-entérologie hépatologie
    - Gendarmerie
    - Géomètre
    - Glacier
    - Greffe des associations
    - Guichet france services
    - Gymnase
    - Gynécologie
    - Hématologie
    - Herboristerie naturopathie
    - Hôpital
    - Horlogerie
    - Hôtel
    - Hôtel restaurant
    - Huissier
    - Hypermarché
    - Hypnothérapeute
    - Immobilier
    - Imprimerie photocopie reliure
    - Infirmier
    - Information Touristique
    - Informatique
    - Institut de formation
    - Instruments et matériel de musique
    - Jardin botanique et/ou zoologique
    - Jardinerie
    - Jeux jouets
    - Jeux vidéo
    - Karaoké
    - Kiosque (théâtre, pizza, journaux)
    - Laboratoire d'analyse médicale
    - Laverie
    - Librairie
    - Lieu de culte
    - Lieu de visite
    - Lingerie sous-vêtements
    - Literie
    - Location articles loisirs et sport
    - Location de matériels
    - Location véhicules
    - Loisirs créatifs
    - Luminaire
    - Lycée
    - Magasin de bois de chauffage
    - Magasin de cbd
    - Magasin de souvenirs
    - Magasin de tissus
    - Mairie
    - Maison départementale des personnes handicapées
    - Maison de santé ou centre de santé
    - Maison de services au public
    - Marché
    - Maroquinerie sellerie articles de voyage
    - Massages
    - Masseur kinésithérapeute
    - Matériel de pêche
    - Médecine du travail
    - Médecin généraliste
    - Menuiserie, ébénisterie
    - Mercerie
    - Meubles ameublement
    - Mission d'accueil et d'information des associations
    - Mission locale pour l'insertion professionnelle et sociale des jeunes
    - Monument historique
    - Motocycle vente et entretien
    - Musée
    - Musique
    - Neurologie
    - Notaire
    - Numérique
    - Office du tourisme
    - Opéra
    - Ophtalmologie
    - Opticien
    - Ordre des avocats
    - Organisation patronale, professionnelle, syndicale
    - Organisme de conseil
    - Orthodontie
    - Orthopédie
    - Orthophonie
    - Orthoptie
    - Ostéopathie
    - Oto-rhino-laryngologie
    - Papeterie, presse, journaux
    - Parc
    - Parc d’attraction
    - Parc des expositions
    - Parfumerie beauté
    - Parking & stationnement
    - Patinoire
    - Pâtisserie
    - Pédiatrie
    - Pédicure-podologue
    - Pépinière
    - Personnes âgées : foyer restaurant
    - Personnes âgées : hébergement
    - Pharmacie
    - Photographie
    - Piscine
    - Plage
    - Plateaux et terrains de jeux extérieurs
    - Plomberie, chauffage
    - Pneumologie
    - Point accueil numerique
    - Point conseil budget
    - Point d'information local dédié aux personnes âgées
    - Point information jeunesse
    - Point justice
    - Poissonnerie / commerce de poissons, crustacés et mollusques
    - Pompes funèbres
    - Port
    - Poterie verrerie céramique
    - Pressing, nettoyage
    - Primeur
    - Produits de terroir
    - Produits surgelés
    - Profession libérale
    - Psychologie, Psychiatrie
    - Psychomotricien
    - Puériculture
    - Radiodiagnostic et imagerie médicale
    - Refuge animalier
    - Rempailleur tapissier chaises fauteuils
    - Réparation auto et de matériel agricole
    - Résidence, foyer
    - Ressourcerie
    - Restaurant
    - Restaurant scolaire
    - Restauration rapide
    - Retouche
    - Retraite
    - Revêtements murs et sols
    - Rhumatologie
    - Sage-femme
    - Salle de combat
    - Salle de concert
    - Salle de danse
    - Salle de jeux
    - Salle de réception
    - Salle des fêtes
    - Salle de spectacle
    - Salle multisports
    - Salle non spécialisée
    - Salles de remise en forme
    - Salle spécialisée
    - Salon de thé
    - Sécurité sociale, mutuelle santé
    - Service ou aide à domicile
    - Services techniques
    - Sex shop
    - Skatepark
    - Soins de beauté
    - Sophrologue
    - Spa
    - Sports et loisirs
    - Sports nautiques
    - Stade
    - Station lavage auto
    - Station service
    - Stomatologie
    - Supérette
    - Supermarché
    - Syndic, gérance immo
    - Tabac
    - Tatouage Piercing
    - Taxi
    - Taxidermie
    - Téléphonie
    - Tennis
    - Textile hors habillement
    - Thalassothérapie
    - Théâtre
    - Toilettes publiques
    - Toiletteur
    - Traiteur
    - Transport
    - Trésorerie
    - Tribunal
    - Université ou école supérieure
    - Urologie
    - Vente à distance
    - Vente d'articles de sport
    - Vente de matériel et équipement industriels
    - Vente de matériel médical
    - Vente de matériel pour piscine
    - Vêtements
    - Vétérinaire

#### Proximité d'un arrêt de transport en commun - Propriété `transport_station_presence`

> *Description : Arrêt de transport en commun à moins de 200 mètres de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Stationnement dans l'établissement - Propriété `stationnement_presence`

> *Description : Des places de stationnement sont disponibles au sein de la parcelle de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Stationnements adaptés dans l'établissement - Propriété `stationnement_pmr`

> *Description : Des places de stationnement adaptées sont disponibles au sein de la parcelle de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Stationnement à proximité de l'établissement - Propriété `stationnement_ext_presence`

> *Description : Des places de stationnement sont disponibles à moins de 200 mètres de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Stationnements adaptés à proximité de l'établissement - Propriété `stationnement_ext_pmr`

> *Description : Des places de stationnement adaptées sont disponibles à moins de 200 mètres de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Chemin extérieur - Propriété `cheminement_ext_presence`

> *Description : L'accès à l'entrée depuis la voirie se fait par un chemin extérieur<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Revêtement extérieur - Propriété `cheminement_ext_terrain_stable`

> *Description : Le revêtement est stable (absence de pavés, gravillons, terre, herbe, sable, ou toute surface non stabilisée)<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Chemin extérieur de plain-pied - Propriété `cheminement_ext_plain_pied`

> *Description : L'accès à cet espace se fait de plain-pied, c'est à dire sans rupture brutale de niveau<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Ascenseur/élévateur - Propriété `cheminement_ext_ascenseur`

> *Description : Existe-t-il un ascenseur ou un élévateur&nbsp;?<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Nombre de marches - Propriété `cheminement_ext_nombre_marches`

> *Description : Combien y'a t'il de marches&nbsp;?<br/>Ex : 0*
- Valeur optionnelle
- Type : nombre entier

#### Marches ou escalier sécurisé(es) - Propriété `cheminement_ext_reperage_marches`

> *Description : Présence de nez de marche contrastés, d'une bande d'éveil à la vigilance en haut de l'escalier et/ou de première et dernière contremarches contrastées<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Sens de circulation de l'escalier - Propriété `cheminement_ext_sens_marches`

> *Description : Sens de circulation des marches ou de l'escalier. Valeurs possibles : montant -> Montant, descendant -> Descendant.<br/>Ex : descendant*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - montant
    - descendant

#### Main courante - Propriété `cheminement_ext_main_courante`

> *Description : L'escalier est équipé d'une ou plusieurs main-courantes<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Rampe - Propriété `cheminement_ext_rampe`

> *Description : Présence d'une rampe fixe ou amovible. Valeurs possibles : aucune -> Aucune, fixe -> Fixe, amovible -> Amovible.<br/>Ex : amovible*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - aucune
    - fixe
    - amovible

#### Pente - Propriété `cheminement_ext_pente_presence`

> *Description : Le chemin est en pente<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Degré de difficulté de la pente - Propriété `cheminement_ext_pente_degre_difficulte`

> *Description : Difficulté de la pente. Valeurs possibles : légère -> Légère, importante -> Importante.<br/>Ex : importante*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - légère
    - importante

#### Longueur de la pente - Propriété `cheminement_ext_pente_longueur`

> *Description : Longueur de la pente. Valeurs possibles : courte -> < 0,5 mètres, moyenne -> entre 0,5 et 2 mètres, longue -> > 2 mètres.<br/>Ex : moyenne*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - courte
    - moyenne
    - longue

#### Dévers - Propriété `cheminement_ext_devers`

> *Description : Dévers ou inclinaison transversale du chemin. Valeurs possibles : aucun -> Aucun, léger -> Léger, important -> Important.<br/>Ex : important*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - aucun
    - léger
    - important

#### Bande de guidage - Propriété `cheminement_ext_bande_guidage`

> *Description : Présence d'une bande de guidage au sol facilitant le déplacement d'une personne aveugle ou malvoyante<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Rétrécissement du chemin - Propriété `cheminement_ext_retrecissement`

> *Description : Un ou plusieurs rétrécissements inférieurs à 90 centimètres du chemin pour atteindre l'entrée<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Entrée facilement repérable - Propriété `entree_reperage`

> *Description : L'entrée de l'établissement est facilement repérable<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Entrée vitrée - Propriété `entree_vitree`

> *Description : La porte d'entrée est vitrée<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Repérage de la vitre - Propriété `entree_vitree_vitrophanie`

> *Description : Des éléments contrastés permettent de visualiser les parties vitrées de l'entrée<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Entrée de plain-pied - Propriété `entree_plain_pied`

> *Description : L'entrée se fait de plain-pied, c'est à dire sans rupture brutale de niveau<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Ascenseur/élévateur - Propriété `entree_ascenseur`

> *Description : Présence d'un ascenseur ou d'un élévateur<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Nombre de marches - Propriété `entree_marches`

> *Description : Nombre de marches de l'escalier<br/>Ex : 0*
- Valeur optionnelle
- Type : nombre entier

#### Repérage des marches - Propriété `entree_marches_reperage`

> *Description : Présence de nez de marche contrastés, d'une bande d'éveil à la vigilance en haut de l'escalier et/ou de première et dernière contremarches contrastées<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Main courante - Propriété `entree_marches_main_courante`

> *Description : L'escalier est équipé d'une ou plusieurs main-courantes<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Rampe - Propriété `entree_marches_rampe`

> *Description : Présence d'une rampe fixe ou amovible. Valeurs possibles : aucune -> Aucune, fixe -> Fixe, amovible -> Amovible.<br/>Ex : amovible*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - aucune
    - fixe
    - amovible

#### Sens de circulation de l'escalier - Propriété `entree_marches_sens`

> *Description : Sens de circulation des marches ou de l'escalier. Valeurs possibles : montant -> Montant, descendant -> Descendant.<br/>Ex : descendant*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - montant
    - descendant

#### Dispositif d'appel à l'entrée - Propriété `entree_dispositif_appel`

> *Description : Présence d'un dispositif comme une sonnette pour signaler sa présence<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Type de dispositif d'appel à l'entrée - Propriété `entree_dispositif_appel_type`

> *Description : Dispositifs d'appels présents. Valeurs possibles : bouton -> Bouton d'appel, interphone -> Interphone, visiophone -> Visiophone.<br/>Ex : ['bouton', 'visiophone']*
- Valeur optionnelle
- Type : liste

#### Balise sonore à l'entrée - Propriété `entree_balise_sonore`

> *Description : Présence d'une balise sonore facilitant son repérage par une personne aveugle ou malvoyante<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Aide humaine - Propriété `entree_aide_humaine`

> *Description : Possibilité d'une aide humaine au déplacement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Largeur de la porte - Propriété `entree_largeur_mini`

> *Description : Largeur minimale de la porte d'entrée<br/>Ex : 0*
- Valeur optionnelle
- Type : nombre entier

#### Entrée spécifique PMR - Propriété `entree_pmr`

> *Description : Présence d'une entrée secondaire spécifique dédiée aux personnes à mobilité réduite<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Y a-t-il une porte ? - Propriété `entree_porte_presence`

> *Description : Présence d'une porte à l'entrée de l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Manoeuvre de la porte - Propriété `entree_porte_manoeuvre`

> *Description : Mode d'ouverture de la porte. Valeurs possibles : battante -> Porte battante, coulissante -> Porte coulissante, tourniquet -> Tourniquet, tambour -> Porte tambour.<br/>Ex : coulissante*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - battante
    - coulissante
    - tourniquet
    - tambour

#### Type de porte - Propriété `entree_porte_type`

> *Description : Type de porte. Valeurs possibles : manuelle -> Manuelle, automatique -> Automatique.<br/>Ex : automatique*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - manuelle
    - automatique

#### Visibilité de la zone d'accueil - Propriété `accueil_visibilite`

> *Description : La zone d'accueil (guichet d'accueil, caisse, secrétariat, etc) est visible depuis l'entrée du bâtiment<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Personnel d'accueil - Propriété `accueil_personnels`

> *Description : Personnel à l'accueil des personnes handicapées. Valeurs possibles : aucun -> Aucun personnel, formés -> Personnels sensibilisés ou formés, non-formés -> Personnels non-formés.<br/>Ex : non-formés*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - aucun
    - formés
    - non-formés

#### Audiodescription - Propriété `accueil_audiodescription_presence`

> *Description : L'établissement propose l'audiodescription.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Liste des équipements pour l'audiodescription - Propriété `accueil_audiodescription`

> *Description : Équipements disponibles<br/>Ex : ['app', 'avec_équipement_occasionnel']*
- Valeur optionnelle
- Type : liste

#### Présence d'équipements d'aide à l'audition et à la communication - Propriété `accueil_equipements_malentendants_presence`

> *Description : Présence de produits ou prestations dédiés aux personnes sourdes ou malentendantes<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Liste des équipements d'aide à l'audition et à la communication - Propriété `accueil_equipements_malentendants`

> *Description : Équipements ou prestations disponibles. Valeurs possibles : bim -> Boucle à induction magnétique fixe, bmp -> Boucle à induction magnétique portative, lsf -> Langue des signes française, lpc -> Langue Française Parlée Complétée (LFPC), sts -> Sous-Titrage ou Transcription Simultanée, autres -> Autres.<br/>Ex : ['bim', 'bmp']*
- Valeur optionnelle
- Type : liste

#### Chemin entre l'entrée principale du bâtiment et l'accueil de l'établissement - Propriété `accueil_cheminement_plain_pied`

> *Description : L'accès à cet espace se fait de plain-pied, c'est à dire sans rupture brutale de niveau<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Ascenseur/élévateur - Propriété `accueil_cheminement_ascenseur`

> *Description : Présence d'un ascenseur ou un élévateur<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Nombre de marches - Propriété `accueil_cheminement_nombre_marches`

> *Description : Nombre de marches de l'escalier<br/>Ex : 0*
- Valeur optionnelle
- Type : nombre entier

#### Repérage des marches ou de l'escalier - Propriété `accueil_cheminement_reperage_marches`

> *Description : Nez de marche contrastés, bande d'éveil à la vigilance en haut de l'escalier et/ou première et dernière contremarches contrastées<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Main courante - Propriété `accueil_cheminement_main_courante`

> *Description : L'escalier est équipé d'une ou plusieurs main-courantes<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Rampe - Propriété `accueil_cheminement_rampe`

> *Description : Présence d'une rampe fixe ou amovible. Valeurs possibles : aucune -> Aucune, fixe -> Fixe, amovible -> Amovible.<br/>Ex : fixe*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - aucune
    - fixe
    - amovible

#### Sens de circulation de l'escalier - Propriété `accueil_cheminement_sens_marches`

> *Description : Sens de circulation des marches ou de l'escalier. Valeurs possibles : montant -> Montant, descendant -> Descendant.<br/>Ex : descendant*
- Valeur optionnelle
- Type : chaîne de caractères
- Valeurs autorisées : 
    - montant
    - descendant

#### Nombre de chambres accessibles à une personne en fauteuil roulant - Propriété `accueil_chambre_nombre_accessibles`

> *Description : Nombre de chambres accessibles à une personne en fauteuil roulant.<br/>Ex : 0*
- Valeur optionnelle
- Type : nombre entier

#### Douche accessible - Propriété `accueil_chambre_douche_plain_pied`

> *Description : La douche est à l'italienne ou équipée d'un bac extra plat.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Siège de douche - Propriété `accueil_chambre_douche_siege`

> *Description : La douche est équipée d'un siège de douche.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Douche sécurisée - Propriété `accueil_chambre_douche_barre_appui`

> *Description : La douche est équipée d'une barre d'appui horizontale.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Toilette sécurisé - Propriété `accueil_chambre_sanitaires_barre_appui`

> *Description : Le toilette est équipé d'une barre d'appui horizontale.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Toilette accessible - Propriété `accueil_chambre_sanitaires_espace_usage`

> *Description : Le toilette dispose d'un espace d'usage à côté de la cuvette.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Visibilité des numéros de chambres - Propriété `accueil_chambre_numero_visible`

> *Description : Les numéros de chambres sont repérables et en relief.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Equipement d'alerte adapté - Propriété `accueil_chambre_equipement_alerte`

> *Description : L'établissement dispose d'un ou plusieurs équipements d'alerte par flash lumineux ou vibration.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Accompagnement spécifique - Propriété `accueil_chambre_accompagnement`

> *Description : Il est proposé un accompagnement personnalisé pour présenter la chambre à un client en situation de handicap, notamment aveugle ou malvoyant.<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Rétrécissement du chemin - Propriété `accueil_retrecissement`

> *Description : Présence d'un ou plusieurs rétrécissements inférieurs à 90 centimètres du chemin pour atteindre la zone d'accueil<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Sanitaires - Propriété `sanitaires_presence`

> *Description : Des sanitaires sont mis à disposition dans l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Sanitaires adaptés - Propriété `sanitaires_adaptes`

> *Description : Des sanitaires adaptés sont mis à disposition dans l'établissement<br/>Ex : True*
- Valeur optionnelle
- Type : booléen

#### Marques ou labels - Propriété `labels`

> *Description : Marque(s) ou label(s) obtenus par l'établissement. Valeurs possibles : autre -> Autre, dpt -> Destination pour Tous, mobalib -> Mobalib, th -> Tourisme & Handicap.<br/>Ex : ['mobalib', 'th']*
- Valeur optionnelle
- Type : liste

#### Famille(s) de handicap concernées(s) - Propriété `labels_familles_handicap`

> *Description : Famille(s) de handicap couverte(s) par ces marques ou labels. Valeurs possibles : auditif -> Handicap auditif, mental -> Handicap mental, moteur -> Handicap moteur, visuel -> Handicap visuel.<br/>Ex : ['moteur', 'visuel']*
- Valeur optionnelle
- Type : liste

#### Registre - Propriété `registre_url`

> *Description : Adresse internet à laquelle le registre est consultable<br/>Ex : https://handicap.gouv.fr/actualites/article/registre-d-accessibilite-obligatoire-un-guide-pour-les-erp*
- Valeur optionnelle
- Type : chaîne de caractères (format `uri`)

#### Conformité - Propriété `conformite`

> *Description : L'établissement a été déclaré conforme à la réglementation<br/>Ex : True*
- Valeur optionnelle
- Type : booléen
