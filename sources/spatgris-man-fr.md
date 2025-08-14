**SpatGRIS**

![](sources/media-fr/media/image1.png){width="2.0157206911636045in"
height="2.0in"}

**Outils pour la spatialisation du son en 2D et 3D**

Développés par le

Groupe de Recherche en Immersion Spatiale

**GRIS**

<http://gris.musique.umontreal.ca/>

  -----------------------------------------------------------------------
  **Directeur:**                      Robert NORMANDEAU
  ----------------------------------- -----------------------------------
  **Programmeur:**                    Gaël LANE LÉPINE

  **Assistants:**                     Nicola GIANNINI
  -----------------------------------------------------------------------

**Manuel**

*SpatGRIS* 3.3.7

*SpeakerView* 0.0.7

*ControlGRIS* 1.4.5

BlackHole 0.6.0

**Avril 2025**

![](sources/media-fr/media/image2.png){width="1.0in" height="1.0in"}

Faculté de musique

![](sources/media-fr/media/image3.png){width="3.7115529308836397in"
height="0.2755905511811024in"}
![](sources/media-fr/media/image4.png){width="1.0211614173228347in"
height="0.3937007874015748in"}

**Table des matières**

[1. Présentation générale
[6](#groupe-de-recherche-en-immersion-spatiale-gris)](#groupe-de-recherche-en-immersion-spatiale-gris)

[1.1. SpatGRIS est un outil de spatialisation
[6](#spatgris-est-un-outil-de-spatialisation-et-de-locaisation)](#spatgris-est-un-outil-de-spatialisation-et-de-locaisation)

[1.1.1. Spatialisation [6](#spatialisation)](#spatialisation)

[1.1.2. Localisation [6](#localisation)](#localisation)

[1.2. SpatGRIS est un enregistreur et un lecteur
[6](#spatgris-est-un-enregistreur-et-un-lecteur)](#spatgris-est-un-enregistreur-et-un-lecteur)

[1.3. SpatGRIS fabrique des configurations de haut-parleurs
[6](#spatgris-produit-des-configurations-de-haut-parleurs)](#spatgris-produit-des-configurations-de-haut-parleurs)

[1.3.1. Configuration DOME
[6](#configuration-dome)](#configuration-dome)

[1.3.2 Configuration CUBE [6](#configuration-cube)](#configuration-cube)

[1.4. Les haut-parleurs peuvent faire partie de la spatialisation et de
la localisation
[6](#les-haut-parleurs-participe-à-la-spatialisation-et-à-la-localisation)](#les-haut-parleurs-participe-à-la-spatialisation-et-à-la-localisation)

[1.5. Les trois composantes de SpatGRIS
[7](#les-trois-composantes-de-spatgris)](#les-trois-composantes-de-spatgris)

[1.6. Qu\'y a-t-il de nouveau et d\'amélioré dans ControlGRIS/SpatGRIS?
[7](#quy-a-t-il-de-nouveau-et-damélioré-dans-controlgrisspatgris)](#quy-a-t-il-de-nouveau-et-damélioré-dans-controlgrisspatgris)

[1.7. Groupe de Recherche en Immersion Spatiale (GRIS)
[8](#groupe-de-recherche-en-immersion-spatiale-gris)](#groupe-de-recherche-en-immersion-spatiale-gris)

[2. INTRODUCTION [8](#introduction)](#introduction)

[2.1. Architecture [8](#architecture)](#architecture)

[2.2. SpatGRIS [9](#spatgris)](#spatgris)

[2.2.1. L\'histoire [9](#lhistoire)](#lhistoire)

[2.2.2. Configuration requise
[9](#configuration-requise)](#configuration-requise)

[2.2.3. Notes d\'installation
[9](#notes-dinstallation)](#notes-dinstallation)

[2.2.4. Accès au microphone
[10](#accès-au-microphone)](#accès-au-microphone)

[2.2.5. Volume de BlackHole à 0 dB
[10](#volume-de-blackhole-à-0-db)](#volume-de-blackhole-à-0-db)

[2.2.6. Nouveaux utilisateurs de BlackHole et de macOS 14 Sonoma
[10](#nouveaux-utilisateurs-de-blackhole-et-de-macos-14-sonoma)](#nouveaux-utilisateurs-de-blackhole-et-de-macos-14-sonoma)

[2.3. ControlGRIS [10](#controlgris2)](#controlgris2)

[2.3.1. L'histoire [10](#lhistoire-1)](#lhistoire-1)

[2.3.2. Configuration requise
[10](#configuration-requise-1)](#configuration-requise-1)

[2.3.3. Notes d\'installation
[11](#notes-dinstallation-1)](#notes-dinstallation-1)

[2.3.4. AU, VST, AAX [11](#au-vst-aax)](#au-vst-aax)

[2.4. Guide de démarrage rapide
[12](#guide-de-démarrage-rapide)](#guide-de-démarrage-rapide)

[3. Connections [14](#connections)](#connections)

[3.1. Connecter la SAN à SpatGRIS
[14](#connecter-la-san-à-spatgris)](#connecter-la-san-à-spatgris)

[3.1.1. Ouvrir SpatGRIS [14](#ouvrir-spatgris)](#ouvrir-spatgris)

[3.1.2. Régler le niveau de sortie
[14](#régler-le-niveau-de-sortie)](#régler-le-niveau-de-sortie)

[3.1.3. Assigner la SAN à BlackHole
[14](#assigner-la-san-à-blackhole)](#assigner-la-san-à-blackhole)

[3.1.4. Multiclient [14](#multiclient)](#multiclient)

[3.2. Connecter ControlGRIS à SpatGRIS
[15](#connecter-controlgris2-à-spatgris)](#connecter-controlgris2-à-spatgris)

[3.2.1. Numérotation des canaux audio et OSC
[15](#numérotation-des-canaux-audio-et-osc)](#numérotation-des-canaux-audio-et-osc)

[3.2.2. Couleurs des sources
[16](#couleurs-des-sources)](#couleurs-des-sources)

[4. ControlGRIS [17](#controlgris2-1)](#controlgris2-1)

[4.1. Introduction [17](#introduction-1)](#introduction-1)

[4.2. Interface graphique
[17](#interface-graphique)](#interface-graphique)

[4.3. Panneau de configuration
[18](#panneau-de-configuration)](#panneau-de-configuration)

[4.3.1. Settings [18](#settings)](#settings)

[MODE [18](#mode)](#mode)

[OSC Port [18](#osc-port)](#osc-port)

[IP Address [18](#ip-address)](#ip-address)

[Nombre des sources [18](#nombre-des-sources)](#nombre-des-sources)

[First Source ID [18](#first-source-id)](#first-source-id)

[4.3.2. Sources [19](#sources)](#sources)

[4.3.3. Contrôleurs [19](#contrôleurs)](#contrôleurs)

[4.4. Vues de la spatialisation
[20](#vues-de-la-spatialisation)](#vues-de-la-spatialisation)

[4.4.1 Vue en mode DOME [20](#vue-en-mode-dome)](#vue-en-mode-dome)

[4.4.2. Spans en mode DOME
[20](#spans-en-mode-dome)](#spans-en-mode-dome)

[4.4.3. Vue en mode CUBE [21](#vue-en-mode-cube)](#vue-en-mode-cube)

[4.4.4. Spans en mode CUBE
[21](#spans-en-mode-cube)](#spans-en-mode-cube)

[4.4.5. Élévation en mode CUBE en mode Normal ou Extended Top
[22](#élévation-en-mode-cube-en-mode-normal-ou-extended-top)](#élévation-en-mode-cube-en-mode-normal-ou-extended-top)

[4.4.6. Élévation en mode CUBE dans les modes Extended Top et Bottom
[22](#élévation-en-mode-cube-dans-les-modes-extended-top-et-bottom)](#élévation-en-mode-cube-dans-les-modes-extended-top-et-bottom)

[4.5. Comment utiliser ControlGRIS
[22](#comment-utiliser-controlgris2)](#comment-utiliser-controlgris2)

[4.5.1. Charger le plugiciel sur une piste
[23](#charger-le-plugiciel-sur-une-piste)](#charger-le-plugiciel-sur-une-piste)

[4.5.2. Sauvegarde des mémoires et enregistrement des automations
[23](#sauvegarde-des-mémoires-et-enregistrement-des-automations)](#sauvegarde-des-mémoires-et-enregistrement-des-automations)

[4.5.3. Rappeler les mémoires
[23](#rappeler-les-mémoires)](#rappeler-les-mémoires)

[4.6. Trajectoires
[24](#trajectoires-abstraites)](#trajectoires-abstraites)

[4.6.1. Sources Link [24](#sources-link)](#sources-link)

[Azimuth-Elevation (DOME) et Azimuth-Distance (CUBE) Links
[24](#azimuth-elevation-dome-et-azimuth-distance-cube-links)](#azimuth-elevation-dome-et-azimuth-distance-cube-links)

[Elevation Links (CUBE mode seulement)
[24](#elevation-links-cube-mode-seulement)](#elevation-links-cube-mode-seulement)

[4.6.2. Types de trajectoires
[25](#types-de-trajectoires)](#types-de-trajectoires)

[Azimuth-Elevation (DOME) et Azimuth-Distance (CUBE) Trajectory Type
[25](#azimuth-elevation-dome-et-azimuth-distance-cube-trajectory-type)](#azimuth-elevation-dome-et-azimuth-distance-cube-trajectory-type)

[Elevation (CUBE seulement) Trajectory Type
[25](#elevation-cube-seulement-trajectory-type)](#elevation-cube-seulement-trajectory-type)

[Realtime [26](#realtime)](#realtime)

[Drawing [26](#drawing)](#drawing)

[Maj-Clic en mode Drawing
[26](#maj-clic-en-mode-drawing)](#maj-clic-en-mode-drawing)

[Activate [27](#activate)](#activate)

[Enregistrement de la trajectoire dans la SAN
[27](#enregistrement-de-la-trajectoire-dans-la-san)](#enregistrement-de-la-trajectoire-dans-la-san)

[4.6.3. Un cas particulier : le pendule
[27](#un-cas-particulier-le-pendule)](#un-cas-particulier-le-pendule)

[4.6.4. Mémoires et trajectoires automatisées
[27](#mémoires-et-trajectoires-automatisées)](#mémoires-et-trajectoires-automatisées)

[5. SpatGRIS [29](#spatgris-1)](#spatgris-1)

[5.1. Introduction [29](#introduction-2)](#introduction-2)

[5.2. SpeakerView [30](#speakerview)](#speakerview)

[5.2.1. Visibilité et raccourcis-clavier
[30](#visibilité-et-raccourcis-clavier)](#visibilité-et-raccourcis-clavier)

[5.2.2. Deux applications distinctes
[30](#deux-applications-distinctes)](#deux-applications-distinctes)

[5.3. Modifier la configuration de haut-parleurs et non la
spatialisation
[31](#modifier-la-configuration-de-haut-parleurs-et-non-la-spatialisation)](#modifier-la-configuration-de-haut-parleurs-et-non-la-spatialisation)

[5.4. Réglages (Settings) [32](#réglages-settings)](#réglages-settings)

[5.5. Contrôles [32](#contrôles)](#contrôles)

[5.6. Le DOME et le CUBE [32](#le-dome-et-le-cube)](#le-dome-et-le-cube)

[5.6.1. DOME [33](#dome)](#dome)

[5.6.2. CUBE [33](#cube)](#cube)

[5.7. Le mode HYBRID: DOME et CUBE dans le même projet
[34](#le-mode-hybrid-dome-et-cube-dans-le-même-projet)](#le-mode-hybrid-dome-et-cube-dans-le-même-projet)

[5.7.1. Qu\'est-ce qui est sauvegardé en mode HYBRID ?
[34](#quest-ce-qui-est-sauvegardé-en-mode-hybrid)](#quest-ce-qui-est-sauvegardé-en-mode-hybrid)

[5.7.2. Quel mode est chargé en fonction de l\'ordre d\'ouverture du
Speaker Setup et du Project?
[34](#quel-mode-est-chargé-en-fonction-de-lordre-douverture-du-speaker-setup-et-du-project)](#quel-mode-est-chargé-en-fonction-de-lordre-douverture-du-speaker-setup-et-du-project)

[5.7.3. Attenuation settings dans le mode CUBE ou HYBRID
[35](#attenuation-settings-dans-le-mode-cube-ou-hybrid)](#attenuation-settings-dans-le-mode-cube-ou-hybrid)

[5.7.4. Conversion de DOME en CUBE et vice versa
[36](#conversion-de-dome-en-cube-et-vice-versa)](#conversion-de-dome-en-cube-et-vice-versa)

[5.7.5. Spatialisation en 2D et 3D
[36](#spatialisation-en-2d-et-3d)](#spatialisation-en-2d-et-3d)

[5.8. Dispositif de haut-parleurs
[37](#dispositif-de-haut-parleurs)](#dispositif-de-haut-parleurs)

[5.8.1. Speaker Setup Edition
[38](#speaker-setup-edition)](#speaker-setup-edition)

[5.8.2. Ordre des haut-parleurs et représentation visuelle
[38](#ordre-des-haut-parleurs-et-représentation-visuelle)](#ordre-des-haut-parleurs-et-représentation-visuelle)

[5.8.3. Exigences minimales
[39](#exigences-minimales)](#exigences-minimales)

[5.8.4. Sorties directes [40](#sorties-directes)](#sorties-directes)

[Sorties directes indépendantes
[40](#sorties-directes-indépendantes)](#sorties-directes-indépendantes)

[Sorties directes spatialisées
[40](#sorties-directes-spatialisées)](#sorties-directes-spatialisées)

[5.8.5. Show Speaker Numbers
[41](#show-speaker-numbers)](#show-speaker-numbers)

[5.9. Sources et Speakers
[42](#sources-et-speakers)](#sources-et-speakers)

[5.9.1. Mute et Solo [43](#mute-et-solo)](#mute-et-solo)

[5.9.2. Indicateurs de crête et réinitialisation
[43](#indicateurs-de-crête-et-réinitialisation)](#indicateurs-de-crête-et-réinitialisation)

[5.10. Les réductions stéréo
[43](#les-réductions-stéréo)](#les-réductions-stéréo)

[5.10.1. STEREO [43](#stereo)](#stereo)

[5.10.2. BINAURAL [44](#binaural)](#binaural)

[5.11. Enregistrement [44](#enregistrement)](#enregistrement)

[6. PLAYER [46](#player)](#player)

[6.1. Effectuer un enregistrement pour le PLAYER
[46](#effectuer-un-enregistrement-pour-le-player)](#effectuer-un-enregistrement-pour-le-player)

[6.2. Ouvrir et lire un projet avec le PLAYER
[46](#ouvrir-et-lire-un-projet-avec-le-player)](#ouvrir-et-lire-un-projet-avec-le-player)

[6.2.1. Ouvrir le Speaker Setup pour l\'écoute
[46](#ouvrir-le-speaker-setup-pour-lécoute)](#ouvrir-le-speaker-setup-pour-lécoute)

[6.2.2. Ouvrir la fenêtre PLAYER et charger les fichiers
[47](#ouvrir-la-fenêtre-player-et-charger-les-fichiers)](#ouvrir-la-fenêtre-player-et-charger-les-fichiers)

[6.2.3. Jouer la pièce [48](#jouer-la-pièce)](#jouer-la-pièce)

[6.2.4. DOME dans CUBE ou CUBE dans DOME
[48](#dome-dans-cube-ou-cube-dans-dome)](#dome-dans-cube-ou-cube-dans-dome)

[6.2.5. Les sorties directes dans le PLAYER
[49](#les-sorties-directes-dans-le-player)](#les-sorties-directes-dans-le-player)

[6.3. Sauvegarder un projet PLAYER
[50](#sauvegarder-un-projet-player)](#sauvegarder-un-projet-player)

[7. Menus [51](#menus)](#menus)

[7.1. Menu File [51](#menu-file)](#menu-file)

[7.2. Menu View [51](#menu-view)](#menu-view)

[7.3. Nommer et sauvegarder
[52](#nommer-et-sauvegarder)](#nommer-et-sauvegarder)

[7.4. Représentations [53](#représentations)](#représentations)

[7.4.1. Représentation 3D [53](#représentation-3d)](#représentation-3d)

[7.4.2. Représentation 2D [54](#représentation-2d)](#représentation-2d)

[7.5. Performance et charge de travail du CPU
[54](#performance-et-charge-de-travail-du-cpu)](#performance-et-charge-de-travail-du-cpu)

[7.6. Menu d\'aide [54](#menu-daide)](#menu-daide)

[8. Addendum [55](#addendum)](#addendum)

[8.1. Descriptions des Sources Link
[55](#descriptions-des-sources-link)](#descriptions-des-sources-link)

[8.1.1. Azimuth-Elevation et Azimuth-Distance
[55](#azimuth-elevation-et-azimuth-distance)](#azimuth-elevation-et-azimuth-distance)

[8.1.2. Elevation (Mode CUBE uniquement)
[56](#elevation-mode-cube-uniquement)](#elevation-mode-cube-uniquement)

[8.2. Descriptions des trajectoires
[57](#descriptions-des-trajectoires)](#descriptions-des-trajectoires)

[8.2.1. Azimuth-Elevation et Azimuth-Distance
[57](#azimuth-elevation-et-azimuth-distance-1)](#azimuth-elevation-et-azimuth-distance-1)

[8.2.2. Elevation (Mode CUBE uniquement)
[58](#elevation-mode-cube-uniquement-1)](#elevation-mode-cube-uniquement-1)

[8.3. Messages OSC dans SpatGRIS
[58](#messages-osc-dans-spatgris)](#messages-osc-dans-spatgris)

[8.4. Messages OSC dans ControlGRIS
[60](#messages-osc-dans-controlgris2)](#messages-osc-dans-controlgris2)

[8.5. Open Stage Control et Lemur
[60](#open-stage-control-et-lemur)](#open-stage-control-et-lemur)

[8.6. Désinstaller [60](#désinstaller)](#désinstaller)

[8.6.1. SpatGRIS [60](#spatgris-2)](#spatgris-2)

[8.6.2. ControlGRIS [60](#controlgris2-2)](#controlgris2-2)

[9. Problèmes connus et avertissements
[61](#problèmes-connus-et-avertissements)](#problèmes-connus-et-avertissements)

[9.1. Problèmes connus [61](#problèmes-connus)](#problèmes-connus)

[9.1.1. SpatGRIS, le plugiciel et SpatGRIS, le logiciel
[61](#spatgris-le-plugiciel-et-spatgris-le-logiciel)](#spatgris-le-plugiciel-et-spatgris-le-logiciel)

[9.1.2. [61](#section)](#section)

[9.1.3. [61](#section-1)](#section-1)

[9.2. Reaper [61](#reaper)](#reaper)

[9.2.1. Pistes mono [61](#pistes-mono)](#pistes-mono)

[9.2.2. Préférences avec Jack
[62](#préférences-avec-jack)](#préférences-avec-jack)

[9.3. Logic Pro [62](#logic-pro)](#logic-pro)

[9.3.1. Une seule sortie Surround
[62](#une-seule-sortie-surround)](#une-seule-sortie-surround)

[9.3.2. Bouton Activate [62](#bouton-activate)](#bouton-activate)

[9.4. Digital Performer 11 et automatisation des mémoires
[62](#digital-performer-11-et-automatisation-des-mémoires)](#digital-performer-11-et-automatisation-des-mémoires)

[9.5. Utilisation de SpatGRIS avec des entrées en direct
[62](#utilisation-de-spatgris-avec-des-entrées-en-direct)](#utilisation-de-spatgris-avec-des-entrées-en-direct)

[10. Conseil et astuces [63](#conseil-et-astuces)](#conseil-et-astuces)

[10.1. Spatialisation acousmatique
[63](#spatialisation-acousmatique)](#spatialisation-acousmatique)

[10.1.1. Console de mixage [63](#console-de-mixage)](#console-de-mixage)

[10.1.2. Station Audio Numérique
[63](#station-audio-numérique)](#station-audio-numérique)

[10.1.3. Dispositif acousmatique
[63](#dispositif-acousmatique)](#dispositif-acousmatique)

[10.1.4. Scénario [64](#scénario)](#scénario)

[10.2. Utilisation du PLAYER sans votre présence
[66](#utilisation-du-player-en-votre-absence)](#utilisation-du-player-en-votre-absence)

[10.3. Le mode HYBRID pour varier les trajectoires
[66](#le-mode-hybrid-pour-varier-les-trajectoires)](#le-mode-hybrid-pour-varier-les-trajectoires)

[Index [68](#index)](#index)

![](sources/media-fr/media/image5.png){width="1.0290091863517061in"
height="1.0236220472440944in"}

# Groupe de Recherche en Immersion Spatiale (GRIS)

Directeur : Robert Normandeau.

Programmeur en chef : Gaël Lane Lépine.

Consultant : Devin Roth, créateur de *BlackHole*.

Assistants : Nicola Giannini.

Anciens programmeurs : Samuel Béland, Olivier Bélanger, Vincent
Berthiaume.

Ancien.nes assistant.es : Simone d'Ambrosio, Theo Mathien, Raphaël
Néron-Baribeau, Ofer Pelz, Dominic Thibault, Alexis Langevin-Tétrault,
Vincent Monastesse, David Ledoux, Yohan Brimicombe, Christophe Lengelé,
Mélanie Frisoli, David Piazza. Gabrielle Caux.

Anciens stagiaires: Ludovic Laffineur, Antoine Landrieu, Nicolas Masson,
Hicheme Ben Gaied.

Le GRIS a reçu des subventions de recherche d\'Hexagram, du CRSH et du
FRQSC depuis 2008 jusqu\'en 2025.

Merci à Yohan Brimicombe pour la création du site web :
http://gris.musique.umontreal.ca

# 1. Présentation générale

## 1.1. SpatGRIS est un outil de spatialisation et de locaisation

*SpatGRIS* fait de la spatialisation et de la localisation. La
spatialisation donne à l\'auditeur l\'impression d\'être entouré par le
son. C\'est une expérience immersive. La localisation est un moyen de
placer un son à un endroit très précis dans l\'espace. Les deux concepts
peuvent être utilisés en même temps dans *SpatGRIS*.

### 1.1.1. Spatialisation 

En utilisant ses deux algorithmes DOME ou CUBE, *SpatGRIS* met en
correspondance les sources sonores - qui proviennent de n\'importe quel
logiciel audio - avec une configuration de haut-parleurs. La position
des sources est fournie par des messages OSC. La spatialisation est
réalisée par un système de haut-parleurs dans un espace physique.

### 1.1.2. Localisation 

Avec **l\'**option des sorties directes (indépendantes ou spatialisées),
*SpatGRIS* permet l\'accès direct aux enceintes, par exemple pour gérer
les subwoofers, pour placer un son sur une enceinte particulière ou pour
utiliser une approche de spatialisation basée sur les canaux
(*channel-based*).

## 1.2. SpatGRIS est un enregistreur et un lecteur

*SpatGRIS* permet d\'enregistrer les sorties des haut-parleurs en mode
spatialisé (DOME ou CUBE) ou en mode à deux canaux (STEREO ou BINAURAL)
dans deux standards - WAV, AIFF - et dans deux formats - Mono Files ou
Interleaved (entrelacé). Avec l\'outil PLAYER, *SpatGRIS* peut jouer
n\'importe quelle œuvre multicanale enregistrée avec lui.

## 1.3. SpatGRIS produit des configurations de haut-parleurs

La configuration des haut-parleurs, *Speaker Setup*, peut adopter la
forme d\'un DOME ou la forme libre d\'un CUBE virtuel.

### 1.3.1. Configuration DOME

Dans le DOME, la distance entre chaque haut-parleur et le centre du DOME
est fixe. Les sources sonores peuvent être spatialisées sur la surface
du DOME.

### 1.3.2 Configuration CUBE

Dans le CUBE, les haut-parleurs peuvent être disposés librement dans
l\'espace. Il n\'y a pas de distance fixe entre les enceintes et le
centre de la configuration. Contrairement aux configurations DOME, les
sources sonores peuvent entrer, traverser et sortir de la configuration.
Les sources sonores qui se trouvent à l\'extérieur de la configuration
peuvent être traitées avec des paramètres d\'atténuation (volume et
filtre).

## 1.4. Les haut-parleurs participe à la spatialisation et à la localisation

Chaque haut-parleur a un numéro unique - que ce soit en mode spatialisé
ou en sortie directe - et peut être utilisé pour ces deux fonctions : la
spatialisation et la localisation, grâce aux nouvelles fonctionnalités
de sortie directe. Un haut-parleur peut faire partie de la
spatialisation et être en même temps une sortie directe. Il s\'agit
d\'une différence conceptuelle majeure par rapport aux versions
précédentes, introduite avec la version 3.

## 1.5. Les trois composantes de SpatGRIS

*SpatGRIS* comporte trois composantes qui sont sauvegardées
indépendamment l\'une de l\'autre : Project, Speaker Setup and Settings.

• Save Project. Un projet est couplé à une œuvre et contient un certain
nombre de sources.

• Save Speaker Setup. Une configuration de haut-parleurs est couplée à
une installation physique placée dans un espace.

• Save Settings. Ces paramètres sont liés à une station de travail
(ordinateur et interface audio), y compris les sorties stéréo utilisées
pour la réduction stéréo.

## 1.6. Qu\'y a-t-il de nouveau et d\'amélioré dans ControlGRIS/SpatGRIS?

• *SpatGRIS* est indépendant de toute interface audio virtuelle, que ce
soit *Jack*, *Enzian* ou *BlackHole*. Celle-ci est au choix de
l\'utilisateur.rice.

• Les sorties directes (*Direct Outs),* ont désormais deux fonctions :
*Independent*, pour les enceintes qui ne font pas partie de la
spatialisation, comme les *subwoofers* ; *Spatialized*, par laquelle le
son peut être envoyé directement à n\'importe quelle enceinte faisant
partie du Speaker Setup.

• Compatibilité avec les dernières versions de macOS, de 10.15
(Catalina) à 14.7 (Sonoma) et les nouvelles machines (M1-M2-M3).

• Compatibilité avec ProTools grâce à l\'ajout du format AAX de
*ControlGRIS.*

• STEREO et BINAURAL peuvent être assignés à n\'importe quelle sortie de
la carte son.

• Plusieurs Speaker Setups et Templates de projets sont désormais
intégrés dans le logiciel.

• *ControlGRIS* et *SpatGRIS* sont disponibles pour Windows.

**Nouveautés :**

***SpatGRIS***

• Version 3.4.0

\- Mise à jour avec JUCE 8

\- Un bouton MUTE général a été ajouté.

• Ajouts et correctifs récents

\- Speaker View: les numéros des haut-parleurs sont automatiquement mis
à jour.

\- La fenêtre 3D qui représente les haut-parleurs et les sources est
maintenant indépendante de *SpatGRIS*. La représentation graphique se
fait maintenant dans *SpeakerView*, sous une interface graphique
nettement améliorée.

\- *SpatGRIS* et *BlackHole* possèdent désormais 256 canaux chacun

\- Mode CUBE : Les réglages d\'atténuation ont un bouton Bypass.

\- Mode CUBE : l\'atténuation Z négative commence au plancher.

\- Réduction stéréo : Les Attenuation settings (les réglages
d\'atténuation) sont fonctionnels dans la réduction stéréo en mode CUBE
ou HYBRID.

\- Attenuation settings: Ils sont sauvegardés avec les projets.

\- Introduction du PLAYER, un outil qui permet à *SpatGRIS* d\'être
utilisé comme un logiciel autonome pour jouer n\'importe quelle pièce
enregistrée par lui sur n\'importe quelle configuration de
haut-parleurs.

\- Le mode CUBE utilise un nouvel algorithme : MBAP (Matrix Based
Amplitude Panning).

\- Les fonctions Mute et Solo sont désormais sauvegardées respectivement
avec les projets ou les Speaker Setups.

\- Speaker Setup Edition en modes CUBE et HYBRID : ajout d\'un paramètre
Global Sound Diffusion.

\- Introduction du mode HYBRID qui combine les algorithmes DOME et CUBE.

\- L\'option Show Numbers a été divisée en Show Source Numbers et Show
Speaker Numbers.

***ControlGRIS2***

• Version 2.0.5

\- Changements majeurs, passage à la version 2.

\- Introduction des trajectoires basées sur l\'analyse du signal selon
différents descripteurs audio.

• Ajouts et correctifs récents

~~- La fenêtre Speaker Setup Edition a été considérablement optimisée.~~

\- Offre la possibilité de placer des signaux en dehors du CUBE sur
l\'axe Z*.*

~~- Meilleure compatibilité des paramètres entre *ControlGRIS* et
*SpatGRIS*.~~

~~- Beaucoup d\'améliorations très pratiques et de changements dans la
terminologie !~~

# 2. INTRODUCTION

Ces instructions supposent que vous connaissez les outils suivants :

• La SAN (Station Audio Numérique) que vous utilisez, compatible avec
les plugiciels AU, VST, VST3 ou AAX.

• Votre interface audio.

## 2.1. Architecture

Le système *SpatGRIS* est composé de trois éléments :

• Le plugiciel *ControlGRIS2* où les trajectoires sont conçues et
enregistrées dans un SAN (ou tout autre dispositif OSC).

• *SpatGRIS* lui-même qui spatialise le son, en fonction de la
configuration des haut-parleurs sélectionnée

• Le dispositif audio virtuel *BlackHole*[^1] qui connecte la SAN à
*SpatGRIS*.

L\'architecture se présente comme suit (l\'audio et l\'OSC fonctionnent
en parallèle):

![](sources/media-fr/media/image6.png){width="4.66875in"
height="3.15in"}

## 2.2. SpatGRIS

*SpatGRIS* est un logiciel autonome qui permet la spatialisation des
sons sur différentes configurations de haut-parleurs, en 2D ou en 3D. Il
peut être utilisé avec l\'interface virtuelle *BlackHole* qui peut
fournir jusqu\'à 256 entrées et sorties. Les trajectoires sont envoyées
à *SpatGRIS* depuis le plugiciel *ControlGRIS2*, ou depuis n\'importe
quel autre logiciel OSC[^2]. La spatialisation audio elle-même est
effectuée par *SpatGRIS* et envoyée à l\'interface audio.

### 2.2.1. L\'histoire

Le développement de *SpatGRIS* a commencé en 2020. Il s\'agit d\'une
version réécrite de *ServerGris* (2018) et de *SpatGRIS2* (2020). La
première version officielle de *SpatGRIS* 3.0.0 a été publiée en août
2021. Il s\'agit de notre premier outil de spatialisation sans
*Jack*[^3] !

### 2.2.2. Configuration requise

Le logiciel a été testé sur les OS suivants :

• macOS de 10.15 Catalina™ à 14.7 Sonoma™.

• Il est natif sur les ordinateurs Apple Silicon M1-M2-M3 (version 3.1.8
et plus).

• Windows™ 10. 11.

### 2.2.3. Notes d\'installation

• Téléchargez la dernière version de *SpatGRIS* à partir de SourceForge
:

[https://sourceforge.net/projects/SpatGRIS3/](https://sourceforge.net/projects/spatgris3/)

*SpatGRIS* pour Mac comprend deux programmes d\'installation dans le
même dossier :

SpatGRIS_v3:

• *SpatGRIS* lui-même.

• *SpeakerView* sous trois versions: Forward (recommandé), Compatibility
et Mobile

• *ControlGRIS2* ou *ControlGRIS22* sous forme de dossier compressé
contenant les différents formats du plugiciel.

BlackHole:

• Le périphérique audio virtuel *BlackHole* qui fournit 64, 128 ou 256
canaux audio entre la SAN et *SpatGRIS*.

Notes pour les utilisateurs de MacOS

• *SpatGRIS*, ainsi que *SpeakerView* et un dossier d\'utilitaires, sont
maintenant installés dans un dossier GRIS, dans le dossier Applications.
Il est possible de renommer le dossier GRIS (pour avoir plusieurs
installations, par exemple), mais il n\'est pas conseillé de renommer
quoi que ce soit à l\'intérieur de ce dossier.

• Pour faciliter la gestion du focus entre *SpeakerView* et *SpatGRIS*,
nous vous recommandons d\'autoriser *SpeakerView* à contrôler votre
ordinateur lorsque cela vous est demandé. Si *SpeakerView* ne le demande
pas, allez dans Réglages système... \> Confidentialité et sécurité \>
Accessibilité, et autorisez *SpeakerView*.

*SpatGRIS, SpeakerView, ControlGRIS22* et *BlackHole* seront mis à jour
séparément. Veuillez-vous inscrire à notre infolettre sur
http://gris.musique.umontreal.ca/ pour être informé.es des mises à jour
~~du logiciel~~ sur notre site web*.*

Deux contrôleurs externes sont disponibles pour *ControlGRIS2* :

• Un patch de Open Stage Control pour *iPad*™.

• Un patch de Lemur[^4] pour *iPad*™.

Un manuel Addendum relatif à ces contrôleurs *iPad* est disponible sur
SourceForge.

*SpatGRIS* pour Windows a un seul programme d\'installation :

• *SpatGRIS* lui-même.

• *ControlGRIS2* et *ControlGRIS22* sous forme de dossier compressé
contenant les différents formats du plugiciel.

Il n\'existe pas de version Windows de *BlackHole*. Pour les
utilisateur.rices de Reaper™, il existe la fonction *ReaRoute*, qui
fonctionne de manière similaire à *BlackHole*, mais uniquement pour
Reaper. Il est possible d\'utiliser *Jack* sous Windows[^5]. Lorsque
*BlackHole* est mentionné dans le manuel, remplacez-le par *ReaRoute* ou
*Jack* lorsque vous utilisez Windows.

### 2.2.4. Accès au microphone

**NOTE : Très important pour les utilisateur.rices de Catalina (10.15)
et plus.**

Assurez-vous que *SpatGRIS* a accès au microphone dans les Préférences
système, Sécurité et confidentialité:

![](sources/media-fr/media/image7.jpg){width="3.752830271216098in"
height="1.36in"}

### 2.2.5. Volume de BlackHole à 0 dB

Après avoir installé ou réinstallé *Blackhole*, assurez-vous que le
volume de *BlackHole* est à 0 dB dans la configuration Audio Midi.

![](sources/media-fr/media/image8.jpg){width="6.248331146106737in"
height="1.5in"}

### 2.2.6. Nouveaux utilisateurs de BlackHole et de macOS 14 Sonoma

NOTE : Les nouveaux utilisateurs de BlackHole sous macOS 14 Sonoma
doivent utiliser la dernière version de l\'installateur de BlackHole
0.6.0.

## 2.3. ControlGRIS2

Il existe désormais deux versions de ControlGRIS. La version 1 demeure
disponible afin d\'assurer la compatibilité avec les projets existants
qui l\'utilisent. Et à partir de 2025, *ControlGRIS2* qui introduit le
traitement de signal. Les deux versions peuvent cohabiter. Ce manuel est
consacré à *ControlGRIS2*. Pour la version 1, consulter le manuel de
*SpatGRIS* 3.3.7.

*ControlGRIS2* est un plugiciel OSC[^6] disponible dans les formats AU,
VST, VST3 et AAX (Mac) et dans les formats VST et AAX (Windows). Ce
plugiciel gratuit et open-source envoie des données OSC à *SpatGRIS*
pour spatialiser plusieurs sources sonores sur une configuration
variable de haut-parleurs. Différents modes de liens entre les sources,
Source Link, et un système de trajectoires sont fournis pour la
spatialisation de sources mono, stéréo et multicanaux (jusqu\'à huit
canaux).

### 2.3.1. L'histoire

Le développement de *ControlGRIS* a commencé en 2019. Il s\'est inspiré
de trois plugiciels plus anciens, *OctoGris* (2010), *ZirkOSC* (2012) et
*SpatGris1*(2017). La première version (1.1.0) a été publiée en avril
2020. La première version (2.0.5) de *ControlGRIS2* a été publiée en
avril 2025.

### 2.3.2. Configuration requise

Le plugiciel a été testé sur les systèmes d\'exploitation et les SAN
suivants :

• macOS de 10.15 Catalina™ à 14.7 Sonoma; Digital Performer™ 10 et 11;
Ableton Live™ 10 et 11; Logic Pro™ 10; Reaper™ 6 et 7; Pro Tools™ 2023.6
et 2024.10.

• Il est natif sur les machines Apple Silicon M1-M2-M3 (version 1.3.2 et
plus).

• Windows™ 10, 11[^7]; Reaper™ 6.

### 2.3.3. Notes d\'installation

Téléchargez la dernière version de *ControlGRIS2* depuis SourceForge
(*ControlGRIS2* est inclus dans le programme d\'installation de
*SpatGRIS*) : <https://sourceforge.net/projects/spatgris3/>

Décompressez le fichier téléchargé. Les différents formats seront
installés à l\'endroit approprié. *ControlGRIS2* apparaît dans le
dossier \"UdeM\" de votre SAN.

### 2.3.4. AU, VST, AAX

Les versions Mac ont été testées de manière intensive, mais les versions
Windows 10 et 11, pas tant que ça !

Les commentaires sont bienvenus.

Voici quelques particularités :

• Utilisez la version AU dans DP et Logic Pro sur Mac

• Utiliser la version VST3 dans Reaper et Live.

• Utilisez la version AAX dans ProTools[^8].

• Pour les autres SAN, consultez leur manuel pour déterminer quelle
version est la meilleure.

## 2.4. Guide de démarrage rapide

*SpatGRIS* reçoit des données *Open Sound Control (OSC)* de
*ControlGRIS2*, pour spatialiser les sons dans une configuration de
haut-parleurs. Le son est envoyé du SAN à *SpatGRIS* via *BlackHole.*

Vous n\'avez pas envie de lire le manuel ? Voici les étapes de base pour
spatialiser une piste stéréo sur une interface audio à 64 sorties.

NOTE : Ajustez la taille de la mémoire tampon à la même valeur dans
votre SAN et dans *SpatGRIS*. Une valeur de 512, voire 1024 et plus est
recommandée.

1\. Ouvrez *SpatGRIS*.

2\. Ouvrez les Settings (menu File) ou cliquez directement sur ceux-ci
dans la barre d\'information et attribuez le périphérique d\'entrée
audio à *BlackHole* 128ch et le périphérique de sortie audio à votre
interface audio (vous ne devez le faire que la première fois). Fermer la
fenêtre.

![](sources/media-fr/media/image9.jpg){width="1.561930227471566in"
height="1.5748031496062993in"}

3\. Ouvrez un Speaker Setup DOME (menu File) ou utilisez celui par
défaut.

4\. Ouvrez votre SAN.

5\. Assignez la sortie audio de votre SAN à *BlackHole* 128ch.

6\. Créez une piste stéréo et assignez les sorties à *BlackHole* 128ch
1-2.

7\. Insérez un plugiciel *ControlGRIS2* sur cette piste et mettez-le en
mode DOME.

8\. Le nombre de sources devrait être déjà initialisé et réglé sur 2 et
le First Source ID réglé sur 1.

9\. Sélectionnez Circular Fully Fixed dans Sources Link et démarrer le
séquenceur.

10\. Jouer avec la Source No. 1 et voir le résultat dans *SpatGRIS*.

11\. La couleur des sources est celle des sources sélectionnées dans
Sources (les points rouges dans cet exemple).

Vous êtes maintenant prêt.e.s à jouer et à enregistrer des automations.

![](sources/media-fr/media/image10.png){width="4.652874015748031in"
height="3.2in"}

![](sources/media-fr/media/image11.png){width="4.933461286089239in"
height="5.05in"}

NOTE : Dans chaque piste du SAN, il est obligatoire que les numéros des
canaux de sortie audio correspondent aux numéros des sources OSC
(définis par le paramètre First Source ID) dans l\'instance de
*ControlGRIS2* correspondante pour que le son soit spatialisé dans
*SpatGRIS*. Si ce n\'est pas le cas, la spatialisation sera silencieuse
ou ne fonctionnera pas correctement.

Des questions ? Des précisions ? Lisez le manuel !

Ce manuel se trouve dans le menu Help :

![](sources/media-fr/media/image12.jpg){width="1.8122222222222222in"
height="0.7in"}

# 3. Connections

## 3.1. Connecter la SAN à SpatGRIS

### 3.1.1. Ouvrir SpatGRIS

La première fois que vous ouvrirez *SpatGRIS*, vous devrez :

• Déterminer le nombre de sources (jusqu\'à 256). 64 suffisent dans la
plupart des cas, mais moins de sources signifient moins de charges pour
le processeur. Vous pouvez également utiliser l\'un des projets inclus
dans le menu File -\> Project Templates.

• Créer un speaker setup ou en utiliser un dans le menu File -\> Speaker
Setup Templates.

Après ces deux premières étapes, sauvegardez le Speaker Setup et le
projet dans un dossier de votre choix. Lors du prochain démarrage de
*SpatGRIS*, le dernier Speaker Setup et le dernier projet enregistré
seront chargés automatiquement.

### 3.1.2. Régler le niveau de sortie

Par défaut, le niveau de sortie de *SpatGRIS* est réglé sur le gain
unitaire : 0,00 dB. Il peut être nécessaire de l\'atténuer ou de
l\'augmenter, surtout si c\'est la première fois que vous essayez le
système !

### 3.1.3. Assigner la SAN à BlackHole

Ouvrez votre SAN et assignez BlackHole comme périphérique de sortie
audio. *BlackHole* devrait être détecté comme n\'importe quelle autre
interface audio disponible dans Core Audio*.* Il est possible
d\'attribuer un certain nombre de canaux actifs en fonction du nombre
défini par la commande Set Sources (icône ±)

![](sources/media-fr/media/image13.png){width="5.008129921259843in"
height="2.2in"}

### 3.1.4. Multiclient

*SpatGRIS* est un logiciel multiclient, ce qui signifie qu\'il peut se
connecter à plusieurs logiciels audios en même temps. Gardez à
l\'esprit, cependant, que son utilisation principale est de spatialiser
les sons provenant d\'un seul SAN et il est plutôt rare que deux SAN
arrivent à cohabiter en même temps. Le logiciel reçoit deux types
d\'informations:

• Signaux audio provenant de *BlackHole*

• Signaux OSC provenant de *ControlGRIS2*.

Les deux signaux sont nécessaires pour la spatialisation du son. Pour
les sorties directes, seul le signal audio est nécessaire.

Si vous n\'utilisez qu\'un seul SAN, il n\'y a pas de problème, mais il
est obligatoire que les numéros des canaux de sortie audio correspondent
aux numéros des sources OSC (définis par le paramètre First Source ID)
dans l\'instance de *ControlGRIS2* correspondante pour que le son soit
spatialisé dans *SpatGRIS*. Si ce n\'est pas le cas, la spatialisation
sera silencieuse ou ne fonctionnera pas correctement. Les choses
deviennent un peu plus compliquées si vous avez l\'intention d\'utiliser
plus d\'un logiciel à la fois...

• *BlackHole* dispose d\'un nombre limité de 256 canaux au total. Si
vous voulez connecter un SAN avec 24 canaux et un autre avec 8 canaux,
gardez à l\'esprit que le second SAN devra être réglé sur les canaux n°
25-32 de *BlackHole* et il sera nécessaire que *ControlGRIS2* utilise
les numéros d\'OSC correspondants*.*

NOTE: Ajustez la taille de la mémoire tampon à la même valeur dans votre
SAN et dans *SpatGRIS*. Une valeur de 512 et plus est recommandée.

## 3.2. Connecter ControlGRIS2 à SpatGRIS

### 3.2.1. Numérotation des canaux audio et OSC

La spatialisation est gérée par *SpatGRIS* qui reçoit les signaux OSC de
*ControlGRIS2*. Il est obligatoire que les numéros des canaux de sortie
audio dans la SAN correspondent aux numéros des sources OSC (définis par
le paramètre First Source ID) dans l\'instance de *ControlGRIS*
correspondante pour que le son soit spatialisé dans *SpatGRIS*.

Dans l\'exemple suivant, trois pistes stéréo (rouge, bleu et vert) sont
assignées aux paires de canaux *BlackHole* 1-2, 3-4 et 5-6. Les trois
instances de *ControlGRIS2* utilisent la même numérotation OSC : 1-2,
3-4 et 5-6.

![](sources/media-fr/media/image14.png){width="4.693333333333333in"
height="5.12in"}

Pour que les choses soient claires, il est recommandé d\'utiliser le
même schéma de couleurs dans la SAN et dans *SpatGRIS*.

![](sources/media-fr/media/image15.png){width="5.018343175853018in"
height="3.3in"}

NOTE: Si, par erreur, vous utilisez les mêmes numéros OSC dans plus
d\'une instance de *ControlGRIS2*, les sources dans *SpatGRIS*
oscilleront entre différentes positions parce qu\'elles recevront deux
(ou plusieurs) positions identiques de différents *ControlGRIS2*. C\'est
un bon indicateur que quelque chose ne va pas.

### 3.2.2. Couleurs des sources

La couleur des sources peut être réglée sur n\'importe quelle valeur en
cliquant sur le carré de couleur. Cela ouvre une fenêtre dans laquelle
vous pouvez définir les paramètres de la couleur. C\'est la couleur que
vous verrez dans la fenêtre 2D ou 3D. Si vous utilisez un grand nombre
de sources, il est recommandé de concevoir votre configuration de
couleurs attentivement.

Après avoir fermé cette fenêtre, vous pouvez attribuer la même couleur à
la source suivante sur la droite en cliquant avec le bouton droit de la
souris sur une couleur. Vous pouvez ainsi attribuer la même couleur à
une paire de sources ou à plusieurs sources contiguës.

![](sources/media-fr/media/image16.jpg){width="2.3622047244094486in"
height="1.968503937007874in"}

# 4. ControlGRIS2

*ControlGRIS2* est un plugiciel OSC qui offre deux possibilités, selon
le mode choisi dans *SpatGRIS*:

• DOME.

• CUBE.

Ces deux modes seront expliqués en détail dans la section *SpatGRIS*.

## 4.1. Introduction

*ControlGRIS2* est un plugiciel de spatialisation OSC. Ce plugiciel
permet de déplacer des sources sonores multicanaux sur un ensemble
variable de haut-parleurs. Plusieurs modes de liaison des sources et un
système de trajectoires sont fournis pour permettre la spatialisation de
sources mono, stéréo, quad, 5.1 ou multicanaux jusqu\'à huit canaux.
*ControlGRIS2* ne gère pas l\'audio, il ne gère que les données qui sont
envoyées à *SpatGRIS*. L\'audio lui-même est envoyé du SAN directement à
*SpatGRIS* via *BlackHole*.

Ce document décrit les instructions d\'utilisation et les fonctions
spécifiques à *ControlGRIS2*. Il est supposé que l\'utilisateur.trice
ait une connaissance suffisante du logiciel hôte et qu\'iel peut
exécuter les fonctions de base pour le configurer.

## 4.2. Interface graphique

L\'interface graphique permet de placer les sources sonores. Elle est
légèrement différente en mode DOME qu\'en mode CUBE. Dans DOME, la
distance étant fixée à 1.00, il n\'y a que les paramètres Azimuth et
Elevation à régler. En CUBE, les trois paramètres, X, Y et Z sont
réglables sur deux fenêtres différentes.

![](sources/media-fr/media/image17.png){width="6.503448162729659in"
height="4.6in"}

## 4.3. Panneau de configuration

Le panneau de configuration donne accès aux différents paramètres du
plugiciel. Ces paramètres sont regroupés sous trois onglets : Sources,
Settings, et Controllers.

![](sources/media-fr/media/image18.jpg){width="4.028694225721785in"
height="1.2in"}

### 4.3.1. Settings

#### MODE

Le mode DOME est basé sur l\'algorithme VBAP conçu par Ville Pulkki.
Dans ce mode, l\'espace est représenté par un dôme où la distance entre
chaque point de la surface et le centre du dôme est égale à 1,00. Le
mode CUBE est basé sur l\'algorithme original MBAP[^9] conçu par Gaël
Lane Lépine. Dans ce mode, l\'espace est représenté par un cube à
l\'intérieur duquel il est possible de concevoir n\'importe quelle
configuration de haut-parleurs.

#### OSC Port

Il s\'agit du numéro de port OSC pour la communication entre
*ControlGRIS2* et *SpatGRIS*. Ils doivent être réglés sur le même. 18032
est la valeur par défaut.

#### IP Address

La valeur par défaut est 127.0.0.1, ce qui correspond à l\'adresse du
dispositif interne (c\'est-à-dire votre ordinateur). Cette valeur peut
être modifiée pour envoyer l\'OSC à un ordinateur externe.

#### Nombre des sources 

Le nombre de sources par piste correspond au nombre de canaux audio de
la piste. Ce nombre est limité à huit canaux (comme dans la plupart des
SAN).

#### First Source ID

Ce numéro doit être unique et différent pour chaque canal audio. Vous
devez utiliser les mêmes numéros pour l\'audio et pour l\'OSC.

Si vous n\'avez que des pistes mono, les numéros sont successifs. Si
vous avez des pistes stéréo, vous n\'aurez que des numéros impairs à
placer ici : 1, 3, 5, etc., car les numéros pairs sont automatiquement
attribués au canal droit de chaque piste stéréo. Et si vous travaillez
avec des fichiers sonores octophoniques, le premier identifiant de
source sera 1, la deuxième piste octophonique commencera à 9, etc.

### 4.3.2. Sources

Sous l\'onglet Sources, il est possible de positionner précisément les
sources en utilisant l\'interface graphique ou les zones de texte. Grâce
à l\'option Sources Placement, il est possible de positionner les
sources à équidistance, dans le sens des aiguilles d\'une montre ou dans
un ordre alternatif. Pour ce faire, il suffit de sélectionner la
répartition souhaitée dans le menu déroulant.

![](sources/media-fr/media/image19.jpg){width="1.6454155730533684in"
height="1.2in"}

De plus, il est possible d\'ajuster manuellement la position de chaque
source en entrant ses coordonnées polaires (DOME) ou cartésiennes
(CUBE). Dans le menu déroulant Source Number, sélectionnez d\'abord le
numéro de la source à déplacer. Ensuite, entrez ses nouvelles
coordonnées.

Dans DOME, Elevation et Azimuth correspondent aux coordonnées polaires
courantes de la source sélectionnée :

![](sources/media-fr/media/image20.jpg){width="4.133858267716535in"
height="1.1811023622047243in"}

Dans CUBE, X, Y et Z correspondent aux coordonnées cartésiennes
courantes de la source sélectionnée :

![](sources/media-fr/media/image21.jpg){width="4.133858267716535in"
height="1.1811023622047243in"}

NOTE : Le positionnement manuel des sources individuelles ne fonctionne
que lorsque le mode Independent est sélectionné dans le menu Sources
Link.

### 4.3.3. Contrôleurs

![](sources/media-fr/media/image22.png){width="4.16in"
height="1.2821292650918634in"}

*ControlGRIS2* peut être manipulé par un contrôleur Open Sound
Control[^10] (OSC) externe. Il existe une interface réalisée pour Open
Stage Control et une autre pour Lemur qui permettent de manipuler les
paramètres de *ControlGRIS2* depuis un *iPad*[^11].

• OSC output plugin ID : pour contrôler différentes instances de
*ControlGRIS2*, chacune doit avoir un ID différent.

• Receive et Send doivent être réglés en fonction des canaux OSC
appropriés (par défaut : 9000 et 8000).

• Les adresses de port IP doivent être définies en fonction de votre
réseau Wi-Fi, qu\'il soit public ou local. L\'ordinateur et le
contrôleur doivent être sur le même réseau. *ControlGRIS2* reçoit
automatiquement l\'adresse d\'entrée de votre réseau.

## 4.4. Vues de la spatialisation

*ControlGRIS2* fonctionne en deux modes différents pour la
spatialisation du son : DOME et CUBE.

### 4.4.1 Vue en mode DOME 

En mode DOME, l\'interface graphique est limitée à Azimuth-Elevation.
Dans ce mode, le son est spatialisé sur la surface du dôme. Alors
qu\'une source placée au centre se trouve en haut du dôme, une source
placée à la périphérie se trouve en bas du dôme.

Le dôme est représenté ici de haut en bas, avec des exemples d\'une
source stéréo à gauche et d\'une source octophonique à droite :

![](sources/media-fr/media/image23.jpg){width="2.5in"
height="1.5173611111111112in"}![](sources/media-fr/media/image24.jpg){width="2.5in"
height="1.521101268591426in"}

### 4.4.2. Spans en mode DOME 

Dans les deux modes, les paramètres de Span sont disponibles pour
l\'azimut et l\'élévation. Le Span permet d\'étendre le signal à une
zone plus large que la source elle-même. En mode DOME, les Spans
ressemblent à un arc de cercle de chaque côté de la source :

![](sources/media-fr/media/image25.jpg){width="2.5in"
height="1.5196850393700787in"}![](sources/media-fr/media/image26.jpg){width="2.0255129046369205in"
height="1.52in"}

### 4.4.3. Vue en mode CUBE

En mode CUBE, l\'interface graphique est divisée en deux écrans :
Azimuth-Distance et Elevation. Le mode CUBE ajoute la distance et permet
de déplacer un son à l\'intérieur ou à l\'extérieur de la configuration
des haut-parleurs (représentée par le carré blanc interne). Le CUBE est
représenté du haut à gauche et de profil à droite (la vue 3D n\'apparaît
que dans *SpatGRIS*). Exemples de sources stéréo et octophonique :

![](sources/media-fr/media/image27.jpg){width="2.5306288276465443in"
height="1.52in"}
![](sources/media-fr/media/image28.jpg){width="2.5043471128608923in"
height="1.52in"}

### 4.4.4. Spans en mode CUBE 

En mode CUBE, les Spans ressemblent à un cylindre entourant la source :

![](sources/media-fr/media/image29.jpg){width="2.4666196412948382in"
height="1.5in"}![](sources/media-fr/media/image30.jpg){width="1.75084208223972in"
height="1.5in"}

Dans certaines configurations CUBE, où la plupart des enceintes sont
réparties sur les murs et le plafond, une source peut être perdue au
centre de la salle. Si vous souhaitez créer un disque sonore plat qui
n\'active que les enceintes situées à la même hauteur que la source,
vous pouvez ajouter un peu d\'Azimuth Span :

![](sources/media-fr/media/image31.jpg){width="6.15in"
height="1.9514424759405073in"}

### 4.4.5. Élévation en mode CUBE en mode Normal ou Extended Top

Depuis la version 1.4.1, *ControlGRIS2* offre la possibilité de placer
une source en dehors du CUBE en élévation. Cela était déjà possible sur
les axes x et y, et c\'est maintenant possible sur l\'axe z également.
Lors de l\'utilisation du mode Extended Top, une ligne horizontale
blanche apparaît dans l\'affichage de l\'élévation. Cette ligne
représente la valeur 1,0 utilisée dans le mode Normal. C\'est à partir
de ce point que les paramètres d\'atténuation de *SpatGRIS* commencent à
prendre effet en élévation. Les sources seront filtrées en volume et/ou
en fréquences à mesure qu\'elles s\'éloignent du sommet du CUBE :

![](sources/media-fr/media/image32.jpg){width="6.15in"
height="1.9126760717410323in"}

### 4.4.6. Élévation en mode CUBE dans les modes Extended Top et Bottom 

Une deuxième ligne apparaît en mode Extended Top et Bottom pour atténuer
les sons envoyés sous le plancher (pour les chanceux qui ont accès à un
cube complet !) La ligne du haut représente la valeur 1.0 du mode
normal. La ligne du bas représente la valeur 0.0 du mode normal :

![](sources/media-fr/media/image33.jpg){width="6.15in"
height="1.9061056430446195in"}

NOTE 1 : Les anciens projets peuvent toujours être utilisés en mode
Normal où la gamme complète de 0.00 à 1.00 est toujours disponible.

NOTE 2 : Il n\'est pas encore possible de descendre sous le sol dans une
sphère complète avec *ControlGRIS2* en mode DOME. Nous y travaillons.
Mais il est possible de le faire en utilisant n\'importe quel logiciel
qui envoie des données OSC directement à *SpatGRIS*.

## 4.5. Comment utiliser ControlGRIS2

*ControlGRIS2* est un plugiciel qui peut être inséré sur n\'importe
quelle piste nécessitant une spatialisation. *ControlGRIS2* comprend un
système de trajectoire qui peut écrire des mouvements prédéfinis
rapidement et efficacement. La fonction d\'automation du logiciel hôte
permet d\'enregistrer et de reproduire les mouvements des sources. Il
est donc essentiel de comprendre les différents modes d\'automation de
votre logiciel hôte préféré.

### 4.5.1. Charger le plugiciel sur une piste

*ControlGRIS2* se charge de la même manière que n\'importe quel autre
plugiciel AU ou VST. Le plus souvent, *ControlGRIS2* est chargé à la fin
de la chaîne des effets de la piste.

NOTE : Dans chaque piste du SAN, il est obligatoire que les numéros des
canaux de sortie audio correspondent aux numéros des sources OSC
(définis par le paramètre First Source ID) dans l\'instance de
*ControlGRIS2* correspondante pour que le son soit spatialisé dans
*SpatGRIS*. Si ce n\'est pas le cas, la spatialisation sera silencieuse
ou ne fonctionnera pas correctement.

### 4.5.2. Sauvegarde des mémoires et enregistrement des automations

Il est possible de sauvegarder certains des paramètres du plugiciel
*ControlGRIS2* dans les 50 plages de mémoire fournies. Les raccourcis
sont les suivants :

• Shift-Click Numéro de mémoire : Save.

• Click Numéro de mémoire : Load.

• Opt[^12]-Click Numéro de mémoire : Delete.

Ces fonctions apparaissent sous la ligne 49-50 :

![](sources/media-fr/media/image34.jpg){width="0.6805555555555556in"
height="0.6527777777777778in"}

Ces mémoires vous permettent d\'enregistrer et de rappeler les
paramètres suivants uniquement :

• Source positions (Azimuth-Distance-Elevation). Ceux-ci peuvent
également être automatisés.

Les paramètres qui ne sont pas enregistrés, mais qui peuvent être
automatisés :

• Spans.

• Sources Link et Sources Link Alt.

• Presets.

• Bypass.

Les paramètres qui ne sont pas sauvegardés et non automatisés, car ils
sont utilisés pour générer automatiquement une trajectoire qui sera
écrite par la SAN lui-même :

• Spans link.

• Trajectory Type.

• Dur per cycle.

• Sec(s)/Beat(s).

• Number of cycles dampening.

• Deviation degrees per cycle.

• Back & Forth.

• Activate.

Configuration tab

• L\'ensemble de l\'onglet Configuration n\'est pas sauvegardé dans la
mémoire (celui-ci est sauvegardé avec le projet SAN). Ce n\'est pas une
bonne idée de modifier ces paramètres à l\'intérieur d\'une piste.

REMARQUE : Bien qu\'il soit possible d\'enregistrer la position de
toutes les sources dans les préréglages, il n\'est possible
d\'enregistrer que l\'automation de la source n° 1 dans le séquenceur.
La source n° 1 est le leader tandis que les autres sources sont des
suiveurs.

### 4.5.3. Rappeler les mémoires

Comme indiqué ci-dessus, les mémoires ne mémorisent que la position des
sources. Lorsqu\'une mémoire est chargée, les sources sont positionnées
en fonction des données stockées. Gardez cependant à l\'esprit que le
séquenceur possède également une mémoire de la position précédente des
sources, et que les deux peuvent interagir de manière étrange. Très
souvent, ce n\'est que lorsque vous démarrez le séquenceur que les
sources prennent leur position réelle. Pour éviter toute ambiguïté, la
sélection des mémoires peut être automatisée.

## 4.6. Trajectoires abstraites

![](sources/media-fr/media/image35.jpg){width="4.133863735783027in"
height="1.1811023622047243in"}

Il est possible d\'automatiser le déplacement des sources sonores à
l\'aide de trajectoires prédéfinies. Dans le panneau de contrôle
Trajectories, vous pouvez définir et ajuster ces mouvements au contexte
musical. Le concept derrière les trajectoires est qu\'il y a une source
leader tandis que les autres sont des suiveurs. Seule la source n° 1
peut être le leader.

Si vous essayez d\'enregistrer l\'automation d\'une autre source que la
source n° 1, vous obtiendrez cet avertissement :

![](sources/media-fr/media/image36.jpg){width="4.133858267716535in"
height="1.105896762904637in"}

### 4.6.1. Sources Link

Le mode Independent n\'est disponible que pour placer initialement les
sources de manière indépendante dans une piste multicanal. Mais la
position des sources ne peut pas être automatisée indépendamment. Seule
l\'automatisation de la source no. 1 peut être enregistrée. Par
conséquent, une fois les sources placées, il est nécessaire de choisir
une autre Sources Link avant d\'enregistrer l\'automation.

#### Azimuth-Elevation (DOME) et Azimuth-Distance (CUBE) Links

Dans la section Trajectories, sous le menu déroulant Sources Link, il
est possible de choisir différentes façons de relier les sources entre
elles. En fonction du nombre de canaux, certains liens peuvent ne pas
être disponibles :

• Mono: seulement Independent.

• Stereo: tous les liens

• Multichannel: tous sauf Symmetric X et Y.

• Des représentations détaillées des liens Azimuth-Elevation et
Azimuth-Distance sont présentées dans l\'Addendum 8.1.1.

![](sources/media-fr/media/image37.jpg){width="4.133858267716535in"
height="1.1811023622047243in"}

#### Elevation Links (CUBE mode seulement)

En mode CUBE, les Elevation Links entre les sources sont indépendants
des paramètres d\'azimut et de distance.

• Des représentations détaillées des Elevation Links sont présentées
dans l\'Addendum 8.1.2.

![](sources/media-fr/media/image38.jpg){width="4.133858267716535in"
height="1.1811023622047243in"}

### 4.6.2. Types de trajectoires

Automatiser le déplacement d\'une source est très simple grâce aux
différents types de trajectoires disponibles.

• Des représentations détaillées des Trajectories sont présentées dans
l'Addendum 8.2.

#### Azimuth-Elevation (DOME) et Azimuth-Distance (CUBE) Trajectory Type

Un menu déroulant vous permet de sélectionner différents types de
trajectoires tels que le cercle, l\'ellipse, la spirale, le carré et le
triangle, dans le sens des aiguilles d\'une montre ou dans le sens
inverse.

![](sources/media-fr/media/image39.jpg){width="4.137795275590551in"
height="2.3332567804024498in"}

#### Elevation (CUBE seulement) Trajectory Type

Un menu déroulant avec différents types de trajectoires vous permet de
choisir parmi une variété de trajectoires telles que Haut-Bas, Bas-Haut.

![](sources/media-fr/media/image40.jpg){width="4.13in"
height="1.249148075240595in"}

Autres paramètres

• La durée de la trajectoire en seconde(s) ou en mesure(s) (beats) (liée
au tempo MIDI du séquenceur hôte).

• Le nombre de cycles d\'amortissement (Number of cycles dampening): la
durée totale = Durée par cycle x Nombre de cycles x 1,5. Le Dampening ne
fonctionne qu\'avec le Back & Forth.

• L'option Back & Forth (aller-retour).

• La déviation en degrés par cycle (The Deviation degrees per cycle.)

#### Realtime

Il s\'agit de l\'enregistrement habituel des automations : vous déplacez
un paramètre (ou plusieurs paramètres) et cela est enregistré dans la
SAN.

#### Drawing

Le mode Drawing vous permet de dessiner une trajectoire directement dans
le plugiciel lui-même. Cette trajectoire peut ensuite être modifiée en
éditant la durée, l\'amortissement et la déviation. Lorsque les
paramètres souhaités sont trouvés, ils peuvent être enregistrés dans la
station de travail audio elle-même.

![](sources/media-fr/media/image41.png){width="5.277777777777778in"
height="3.5in"}

Le mode Drawing est un mode à main levée. Lorsque vous le sélectionnez,
une croix gris pâle apparaît, avec laquelle vous dessinez une
trajectoire. La durée de la trajectoire et le dessin sont temporairement
stockés dans le plugiciel. Dans Azimuth-Elevation (DOME) ou
Azimuth-Distance (CUBE), c\'est la position qui est enregistrée. En
élévation (CUBE uniquement), c\'est la position dans le temps qui est
enregistrée. Les deux fenêtres partagent un cycle qui peut être modifié
à l\'aide des paramètres habituels. Pour voir la trajectoire en action,
vous pouvez activer les boutons Activate et jouer la séquence. Lorsque
le séquenceur s\'arrête, les boutons d\'activation redeviennent éteints.
Des modifications peuvent être apportées, puis il est possible
d\'activer à nouveau Activate. Une fois satisfait du résultat, il est
possible d\'enregistrer la trajectoire dans la SAN.

#### Maj-Clic en mode Drawing 

En appuyant sur la touche Maj en mode Drawing, il est possible de
dessiner des lignes droites ou des figures géométriques irrégulières
dans la fenêtre Azimuth-Elevation (DOME) ou Azimuth-Distance (CUBE).
Chaque fois que vous cliquez, un nouvel angle est créé. N\'oubliez pas
de cliquer une dernière fois lorsque vous avez terminé !

![](sources/media-fr/media/image42.jpg){width="1.3186154855643044in"
height="1.4015748031496063in"}![](sources/media-fr/media/image43.jpg){width="1.3130435258092739in"
height="1.4in"}

NOTE: Attention à la trajectoire à main levée, car elle est temporaire.
Si vous cliquez n\'importe où dans la fenêtre après avoir dessiné une
trajectoire, ou si vous fermez le plugiciel ou la session, elle sera
automatiquement effacée. Un seul geste peut être enregistré
temporairement à la fois. La croix X pourrait être cachée derrière
l\'une des sources. Il suffit de déplacer l\'une d\'entre elles pour la
retrouver.

#### Activate

![](sources/media-fr/media/image44.jpg){width="4.120431977252843in"
height="1.1811023622047243in"}

En appuyant sur le bouton Activate, *ControlGRIS2* attend le démarrage
du séquenceur. Lorsque la séquence est lancée, le plugiciel démarre la
trajectoire selon les paramètres spécifiés. Le mouvement produit peut
être enregistré --- coordonnées X, Y et Z de la source n° 1 --- comme
toute autre automatisation. Lorsque le séquenceur s\'arrête, les boutons
d\'activation reviennent à l\'état OFF. Il est important de placer la
tête de lecture dans la bonne position avant d\'appuyer sur le bouton
Activate et de lancer la séquence.

#### Enregistrement de la trajectoire dans la SAN

Comme expliqué ci-dessus, *ControlGRIS2* attend que le séquenceur hôte
démarre avant de commencer une trajectoire. Les pistes qui contiennent
*ControlGRIS2* peuvent être configurées en mode d\'écriture (Touch,
Latch ou Write --- selon les options de votre SAN) pour enregistrer les
mouvements des sources comme automations. Ces automations sont alors
disponibles pour la lecture et l\'édition.

NOTE: Seule la source n°1 (leader) est enregistrée, les autres sources
étant des suiveurs. Il est toujours préférable d\'enregistrer les
automations de trajectoires dans la SAN après avoir trouvé les bons
réglages, car cela libère le CPU utilisé par *ControlGRIS2*.

### 4.6.3. Un cas particulier : le pendule

Une utilisation spécifique du Shift-Click en mode Drawing peut être
utilisée pour concevoir un pendule. Si une simple ligne est tracée avec
Shift-Click, elle constitue l\'élément de base d\'un pendule. Ensuite,
les fonctions Dur per cycle, Dampening, Deviation et Back & Forth
peuvent être utilisées pour rendre ce pendule très intéressant. Il peut
être placé n\'importe où dans l\'espace.

![](sources/media-fr/media/image45.jpg){width="1.2904232283464567in"
height="2.3622047244094486in"}

### 4.6.4. Mémoires et trajectoires automatisées

Il est possible d\'enregistrer la sélection des mémoires dans le
séquenceur. Mais pour éviter des informations contradictoires entre les
trajectoires automatisées et les presets automatisés (qui mémorisent la
position x-y des sources), dans l\'enregistrement de l\'automation, les
coordonnées x et y, enregistrées dans la mémoire, seront automatiquement
inscrites dans les courbes x-y de l\'automation. Les mémoires
automatisées sont conçues essentiellement pour offrir la possibilité
d\'appliquer des changements soudains dans la position des sources.

![](sources/media-fr/media/image46.png){width="5.67213145231846in"
height="3.46in"}

NOTE: Soyez prudent. Si vous écrasez les automations X et Y existantes,
elles risquent d\'entrer en conflit avec les informations enregistrées
dans les mémoires. Vous obtiendrez alors certainement des anomalies
audios.

## 4.7. Trajectoires concrètes

La grande nouveauté de ControlGRIS2 est la possibilité de générer des
trajectoires à partir de l\'analyse du signal audio qu\'on veut
spatialiser.

# 5. SpatGRIS 

• *SpatGRIS* fait de la spatialisation et de la localisation.

• *SpatGRIS* est un enregistreur et un lecteur.

• *SpatGRIS* fabrique des dispositifs de haut-parleurs.

## 5.1. Introduction

*SpatGRIS* comporte trois composantes qui sont sauvegardées de manière
indépendante : Project, Speaker Setup et Settings.

• **Save Project**. Un projet est couplé à une œuvre qui contient un
certain nombre de sources (sorties du SAN) et le Mode utilisé. C\'est le
composant en haut à droite de *SpatGRIS*.

• **Save Speaker Setup**. Un speaker setup est couplé à une installation
placée dans un espace et à l\'algorithme utilisé. C\'est la section qui
est montrée dans *SpeakerView*.

• **Save Settings**. Les réglages de l\'utilisateur sont liés à une
station de travail --- ordinateur et interface audio --- y compris les
sorties stéréo utilisées pour la réduction stéréo (même sans les
afficher). La plupart des paramètres sont affichés dans la barre
d\'information. Cliquez sur la barre d\'information ou sur Settings dans
le menu File (Cmd-,).

NOTE: Les modes DOME et CUBE sont sauvegardés dans les Speaker Setup et
les Projects, mais le mode HYBRID n\'est sauvegardé que dans les
projets. Le dernier document ouvert --- qu\'il s\'agisse d\'un Speaker
Setup ou d\'un Project --- détermine le Mode.

La fenêtre de *SpatGRIS* est divisée en différentes zones :

• Sources

• VU Meters.

• Settings et Info.

• Controls.

• Recording.

*SpeakerView* affiche les haut-parleurs dans la vue 3D.

![](sources/media-fr/media/image47.png){width="6.5in"
height="3.7652438757655293in"}

## 5.2. SpeakerView

À partir de la version 3.3.3 de *SpatGRIS*, la représentation 3D des
haut-parleurs est prise en charge par une application indépendant qui se
nomme *SpeakerView* Ce changement a été nécessaire afin de satisfaire
aux exigences des processeurs Apple Silicon pour Mac. Tout est mieux
ici: la transparence des haut-parleurs, la lisibilité des chiffres et la
fluidité des mouvements ont été améliorés de manière spectaculaire.

*SpeakerView* est montré ici avec la nouvelle fonction Show Hall:

![](sources/media-fr/media/image48.png){width="3.3246555118110237in"
height="3.0in"}

### 5.2.1. Visibilité et raccourcis-clavier

*SpeakerView* s\'affiche indépendamment de *SpatGRIS*. Par défaut, il
s\'affiche en même temps que ce dernier. Mais il peut être ouvert ou
fermé de manière indépendante (Mac: Opt-V; Windows: Alt-V).

Les raccourcis claviers présents dans le menu View de *SpatGRIS*
contrôlent les options d\'affichage dans *SpeakerView*:

![](sources/media-fr/media/image49.jpg){width="1.6in"
height="2.388807961504812in"}

### 5.2.2. Deux applications distinctes

Bien que *SpeakerView* ressemble à la représentation 3D qui existait
dans les versions de SpatGRIS antérieures à 3.3.0, il s\'agit d\'une
application distincte. On peut la déplacer et la dimensionner de manière
indépendante. On peut aussi décider de la forcer à rester au premier
plan par rapport à *SpatGRIS* (Keep SpeakerView On Top).

NOTE : *SpeakerView* est une application autonome, mais l\'utilisateur
n\'a pas à s\'en préoccuper, *SpatGRIS* s\'occupera de tout. Nous
recommandons même fortement de ne pas lancer *SpeakerView* à partir du
Finder ou du Dock. S\'il est ouvert de cette manière, voici le message
d\'avertissement qui s\'affichera :

![](sources/media-fr/media/image50.jpg){width="1.222561242344707in"
height="1.0in"}

## 5.3. Modifier la configuration de haut-parleurs et non la spatialisation

La caractéristique la plus intéressante de *SpatGRIS* est que les
Sources, qui proviennent du SAN et représentent l\'audio et la
spatialisation de votre travail, sont indépendantes des haut-parleurs.
Ainsi, si vous avez initialement défini une structure de spatialisation
très complexe pour une configuration de haut-parleurs spécifique, vous
pouvez la jouer sur n\'importe quelle autre configuration de
haut-parleurs par la suite, en particulier en mode DOME. Il vous suffit
de changer la configuration des enceintes d\'un endroit à l\'autre.

Voici un exemple d\'une pièce conçue pour un système de 16 enceintes (à
gauche), présentée sur un système de 24 enceintes totalement différent
(à droite), en passant simplement d\'un système à l\'autre.

Comme vous pouvez le voir, toutes les sources restent exactement aux
mêmes coordonnées. Elles seront jouées par des enceintes différentes,
mais entendues au même endroit dans la salle de concert.

![](sources/media-fr/media/image51.jpg){width="2.522309711286089in"
height="3.1496062992125986in"}![](sources/media-fr/media/image52.jpg){width="2.5229166666666667in"
height="3.1493055555555554in"}

## 5.4. Réglages (Settings)

![](sources/media-fr/media/image9.jpg){width="1.952412510936133in"
height="1.968503937007874in"}

Audio Settings

• Audio device type: Core Audio (default).

• Audio input device: *BlackHole* (idéalement).

• Audio output device: votre interface audio.

• Sampling Rate (Hz): de 44100 à 192000, selon votre interface audio.

• Buffer Size (spls): from 16 to 2048. Ajustez la taille de la mémoire
tampon à la même valeur dans votre SAN et dans *SpatGRIS*.

General Settings:

• OSC Input Port: la valeur par défaut est 18032, ce qui correspond à
celle de *ControlGRIS2*. Si vous souhaitez utiliser un autre dispositif
OSC entrant, utilisez ce numéro de port comme port de sortie de ce
dispositif, sinon vous devez modifier ce numéro en conséquence.

**Close**

Vos paramètres sont automatiquement sauvegardés. Sous le nom de la
version de *SpatGRIS*, le document se trouve ici (Mac) :

• \~/Bibliothèque/Application Support/GRIS/SpatGRIS.0.0 (par exemple).

## 5.5. Contrôles

![](sources/media-fr/media/image53.png){width="6.415094050743657in"
height="3.0in"}

## 5.6. Le DOME et le CUBE

En mode DOME, il est possible de placer les sources sur la surface du
dôme formé par les enceintes, tandis qu\'en mode CUBE, il est possible
de déplacer et de placer les sources à l\'intérieur et à l\'extérieur du
speaker setup.

### 5.6.1. DOME

Le DOME, basé sur le VBAP (Vector Base Amplitude Panning), permet à
l\'utilisateur de spatialiser le son sur un dôme de haut-parleurs en
fonction de l\'amplitude relative de trois haut-parleurs (par opposition
à deux dans le panoramique stéréo). Le dôme est donc constitué de
triangles de haut-parleurs. De cette manière, le son peut se propager de
manière fluide sur la surface du dôme, sans bosses ni trous.

Il est possible de voir les triangles en choisissant Show Speaker
Triplets (Opt-T) dans le menu View. Si vous avez la chance d\'utiliser
une sphère complète, il est possible de l\'afficher (Opt-O) !

![](sources/media-fr/media/image54.jpg){width="2.982509842519685in"
height="2.35in"}![](sources/media-fr/media/image55.jpg){width="2.480658355205599in"
height="2.35in"}

### 5.6.2. CUBE

Depuis la version 3.2.0, le mode CUBE est basé sur l\'algorithme MBAP
(Matrix Base Amplitude Panning) et permet de placer une source
n\'importe où dans un espace représenté par un cube. Mais il n\'est pas
limité à la forme d\'un cube. Toute configuration de haut-parleurs peut
être placée dans un cube (y compris un dôme !). Par conséquent, toute
installation sonore ou situation de concert peut être simulée ici. En
mode CUBE, la distance d\'une source sortant du speaker setup est prise
en compte pour simuler le comportement naturel du son qui s\'éloigne.

Comme son nom l\'indique, l\'algorithme est basé sur une matrice
tridimensionnelle précalculée de plusieurs points par haut-parleur qui
détermine l\'amplitude d\'une source à une position spécifique.

![](sources/media-fr/media/image56.jpg){width="3.0342858705161855in"
height="2.36in"}![](sources/media-fr/media/image57.jpg){width="2.1369444444444445in"
height="2.36in"}

## 5.7. Le mode HYBRID: DOME et CUBE dans le même projet

Le mode HYBRID n\'est pas vraiment un nouvel algorithme, mais une
combinaison des algorithmes DOME et CUBE. Le mode HYBRID peut être
sélectionné dans la section Algorithm :

![](sources/media-fr/media/image58.jpg){width="1.6041666666666667in"
height="0.5in"}

Le menu Sources est alors modifié pour offrir la possibilité de choisir
entre le comportement dôme ou cube indépendamment pour chaque source :

![](sources/media-fr/media/image59.jpg){width="2.486842738407699in"
height="0.9in"}

Le mode HYBRID utilise l\'algorithme DOME, ce qui signifie que la
configuration des enceintes doit être un dôme (si ce n\'est pas le cas,
il vous sera demandé de le convertir) à l\'intérieur duquel les sources
peuvent être déplacées selon les comportements CUBE où il est possible
de déplacer le son à l\'intérieur ou à l\'extérieur du dôme de
haut-parleurs. En mode HYBRID, les spans conservent leur comportement
habituel du mode dôme ou du mode cube.

### 5.7.1. Qu\'est-ce qui est sauvegardé en mode HYBRID ?

Deux types d\'informations sont enregistrés avec un projet en mode
HYBRID :

• Le mode HYBRID lui-même est sauvegardé exclusivement avec le projet.

• La sélection de l\'algorithme DOME ou CUBE pour chaque source est
également sauvegardée avec le projet.

Si un ancien projet HYBRID (antérieur à la version 3.1.8) est ouvert en
mode DOME ou CUBE, les sélections concernant les sources n\'apparaîtront
pas. Il faudra choisir manuellement le mode HYBRID pour les voir
apparaître. Mais si vous avez déjà ouvert un speaker setup HYBRID, elles
s\'afficheront automatiquement.

### 5.7.2. Quel mode est chargé en fonction de l\'ordre d\'ouverture du Speaker Setup et du Project?

En règle générale, c\'est toujours le dernier document ouvert ---
Speaker Setup ou Project --- qui détermine l\'algorithme utilisé par
*SpatGRIS*.

Un Speaker Setup (SS) suivi d\'un Project (P) :

1.1. SS Dome + P Dome = Dome.

2.1. SS Cube + P Cube = Cube.

3.1. SS Dome + P Cube = Cube. Le dôme SS est converti dans un SS cube.
La forme du SS ne change pas, puisque l\'algorithme du Cube accepte tous
les dômes (ceci peut être confirmé en ouvrant la fenêtre Speaker Setup
Edition). Avant de fermer le SS, il vous sera demandé de sauvegarder les
modifications.

4.1. SS Cube + P Dome = Dome. Le SS cube est converti en dôme après
l\'approbation du message de conversion.

5.1. SS Dome + P Hybrid = Hybrid.

6.1. SS Cube + P Hybrid = Hybrid. Le SS Cube est converti en Dôme après
approbation du message de conversion.

Dans l\'ordre inverse :

1.2. P Dome + SS Dome = Dome.

2.2. P Cube + SS Cube = Cube.

3.2. P Cube + SS Dome = Dome. Le projet Cube a été transformé en Dome.

4.2. P Dome + SS Cube = Cube. Le projet Dome a été transformé en Cube.

5.2. P Hybrid + SS Dome = Hybrid. C\'est la seule exception où Hybrid
est prioritaire, bien qu\'il ait été chargé en premier. C\'est parce que
les projets hybrides ne fonctionnent que sur les SS Dome.

6.2. P Hybrid + SS Cube = Cube. Hybrid disparaît de la vue puisque nous
venons de passer à Cube. C\'est normal. En sélectionnant ensuite
manuellement Hybrid, le SS Cube est converti en Dôme après
l\'approbation du message de conversion. Les informations sauvegardées
du P Hybrid sont alors récupérées.

### 5.7.3. Attenuation settings dans le mode CUBE ou HYBRID 

Dans les modes CUBE et HYBRID, il y a un cercle intérieur et un cercle
extérieur au milieu du Speaker Setup. Dans le cercle intérieur,
l\'atténuation et/ou le filtrage ne sont pas appliqués. En dehors du
cercle intérieur, l\'atténuation et/ou le filtrage peuvent être
appliqués pour simuler la disparition d\'un son qui s\'éloigne. Au
cercle extérieur, l\'atténuation et le filtrage atteignent leurs valeurs
maximales. Vous pouvez indiquer ces valeurs maximales dans les menus
Attenuation settings. En mode HYBRID, les Attenuation settings ne
fonctionnent que pour les sources CUBE.

![](sources/media-fr/media/image60.png){width="2.6894739720034995in"
height="3.5in"}

En fait, le cercle intérieur est une sphère à l\'intérieur de laquelle
les paramètres d\'atténuation commencent à être calculés à partir du
\"plancher\", c\'est-à-dire à partir des coordonnées (0,0, 0,0) :

![](sources/media-fr/media/image61.jpg){width="2.7in"
height="2.5589424759405075in"}

Les paramètres Attenuation settings :

![](sources/media-fr/media/image62.jpg){width="3.0in"
height="0.7980774278215224in"}![](sources/media-fr/media/image63.jpg){width="3.0in"
height="0.8in"}

![](sources/media-fr/media/image64.jpg){width="3.0in"
height="1.1916666666666667in"}![](sources/media-fr/media/image65.jpg){width="3.0in"
height="1.19in"}

• On/Off

• Volume (dB): de 0 à -72, par paliers de -12 dB.

• Filtrage (Hz): de 125 à 16000, par paliers d'octaves.

• Le volume et le filtrage sont indépendants.

• En élévation, l\'atténuation commence en haut (Extended Top) et en bas
(Extended Top and Bottom) du cube.

• Les Attenuation settings fonctionnent également en mode STEREO et
BINAURAL.

NOTE : les Attenuation Settings sont enregistrés dans le projet.

### 5.7.4. Conversion de DOME en CUBE et vice versa

Dans le cas du passage de DOME à CUBE, *SpatGRIS* utilise les
coordonnées XYZ du Speaker Setup pour garder l\'intégrité du Speaker
Setup. Cela ne s\'applique pas au passage de CUBE à DOME, puisque dans
l\'algorithme VBAP, la distance est toujours ajustée à 1,00.
L\'élévation et la distance n\'ont pas le même comportement dans les
algorithmes DOME et CUBE. Un Speaker Setup conserve son apparence et ses
coordonnées XYZ lors de la transition de l\'algorithme DOME à
l\'algorithme CUBE, mais pas l\'inverse.

### 5.7.5. Spatialisation en 2D et 3D

*SpatGRIS* est capable de spatialiser en 2D et 3D en mode DOME ou CUBE.
Il peut être utile d\'utiliser *SpatGRIS* en 2D avec des SANs qui sont
uniquement stéréo comme Ableton Live et Pro Tools native. Cela donne à
ces SANs stéréo la possibilité de gérer des environnements
multienceintes comme les standards du cinéma. Mais bien sûr, la vraie
puissance de *SpatGRIS* réside dans ses capacités 3D.

Les images suivantes présentent un exemple de configuration de
haut-parleurs en 2D --- une octophonie --- et une configuration en 3D
--- un cube de 24 (3x8) haut-parleurs.

![](sources/media-fr/media/image66.jpg){width="2.7389566929133857in"
height="2.3622047244094486in"}![](sources/media-fr/media/image67.jpg){width="2.594757217847769in"
height="2.3622047244094486in"}

## 5.8. Dispositif de haut-parleurs

La conception d\'un dispositif de haut-parleurs est la première étape du
processus. Elle s\'effectue dans la fenêtre *Speaker Setup Edition*
(menu View, Opt-W).

Un menu Templates est fourni avec différents Speaker Setup au format
DOME ou CUBE. Les Speaker Setup dans les Templates ne peuvent pas être
modifiés. Vous pouvez les utiliser, les éditer et les sauvegarder sous
le nom de votre choix en utilisant Save Speaker Setup As dans le menu
File.

![](sources/media-fr/media/image68.jpg){width="2.0646391076115487in"
height="1.5in"}

### 5.8.1. Speaker Setup Edition

![](sources/media-fr/media/image69.png){width="5.9in"
height="3.5474693788276466in"}

Depuis l\'introduction du MBAP (à partir de la version 3.20) en mode
CUBE, le paramètre Global Sound Diffusion permet de modifier la
diffusion du son de manière globale pour l\'ensemble des haut-parleurs.
Une localisation précise est obtenue avec une petite valeur, des valeurs
plus élevées donneront une image spatiale floue. Ce paramètre peut
également influencer la fluidité des trajectoires.

À l\'exception de la distance, qui est fixée à 1,00 en mode DOME (par
définition), les paramètres de speaker setup peuvent être définis par
des valeurs polaires dans DOME (Azimuth, Elevation) ou par des valeurs
cartésiennes dans CUBE (X, Y, Z). En mode DOME, les valeurs cartésiennes
sont grisées. En mode CUBE, les valeurs polaires sont grisées.

### 5.8.2. Ordre des haut-parleurs et représentation visuelle

En cliquant en haut de chaque colonne (sauf pour Gain et Highpass) dans
la fenêtre Speaker Setup Edition, l\'ordre des haut-parleurs peut être
organisé. La colonne la plus importante est celle de la sortie, dans
laquelle vous pouvez déplacer manuellement ou automatiquement chaque
haut-parleur. Cet ordre sera reflété dans l\'ordre des VU-mètres des
haut-parleurs.

Ordre consécutif :

![](sources/media-fr/media/image70.jpg){width="4.724409448818897in"
height="1.4173228346456692in"}

Ordre pair et impair suivi de sorties directes :

![](sources/media-fr/media/image71.jpg){width="4.724409448818897in"
height="1.3537259405074367in"}

Voici un exemple d\'ordre des haut-parleurs qui représente la position
réelle des haut-parleurs dans un studio par rapport à l\'axe Y (voir
5.9.1 pour plus d\'informations). On peut voir sur la section VU-mètre
des haut-parleurs comment l\'énergie est distribuée de la gauche vers la
droite dans le dôme. Les enceintes 11 et 20 sont au centre, et les subs
à l\'extrême gauche et droite, comme dans un studio. Toutes les autres
enceintes sont également réparties le long de l\'axe Y :

![](sources/media-fr/media/image72.jpg){width="6.25in"
height="2.02457239720035in"}

### 5.8.3. Exigences minimales

Le DOME, en particulier, a besoin de conditions minimales pour effectuer
les calculs VBAP. Si la configuration du haut-parleur ne répond pas à
ces exigences, vous serez averti par un ou deux de ces messages :

![](sources/media-fr/media/image73.jpg){width="3.0in"
height="1.0in"}![](sources/media-fr/media/image74.jpg){width="3.0in"
height="1.0in"}

### 5.8.4. Sorties directes

Une source sonore peut être envoyée directement à un haut-parleur via
une sortie directe. Il existe deux types de sorties directes dans
*SpatGRIS*, ce qui n\'était pas le cas auparavant.

#### Sorties directes indépendantes

![](sources/media-fr/media/image75.jpg){width="0.38819444444444445in"
height="1.9680555555555554in"}Il existe des sorties directes
indépendantes destinées à des utilisations spéciales comme les
subwoofers. Ces enceintes sont identifiées par un rectangle orange dans
la fenêtre Speaker Setup Edition.

![](sources/media-fr/media/image76.jpg){width="5.9in"
height="0.533267716535433in"}

Leur placement dans la configuration n\'est pas très important,
puisqu\'elles sont indépendantes de la spatialisation, mais si vous avez
l\'intention de mixer votre projet dans un format à deux canaux, leur
son sera placé dans l\'image stéréo en fonction de leur position
gauche-droite. Ils sont représentés en noir dans la vue 3D des
enceintes.

![](sources/media-fr/media/image77.jpg){width="6.180555555555555in"
height="1.3888888888888888in"}

#### Sorties directes spatialisées

Il s\'agit d\'une nouvelle fonctionnalité de *SpatGRIS*. Tout
haut-parleur de la configuration peut être utilisé comme sortie directe
et continuer à être utilisé par les algorithmes de spatialisation.
Chaque source a une zone de texte de sortie directe qui est vide par
défaut. N\'importe quel numéro de haut-parleur peut y être placé. La
différence entre les types de sortie directe est que les sorties
indépendantes ne sont utilisées qu\'à cette fin. Il n\'y a pas de
distinction dans la vue 3D du haut-parleur pour les sorties directes
spatialisées.

Les sorties directes spatialisées ont été créées par Samuel Béland, une
amélioration majeure de *SpatGRIS*.

On peut voir la distinction lors de la sélection d\'une sortie directe.
Les premiers chiffres, en haut de la colonne (17-18) sont des sorties
directes indépendantes. Les autres numéros (1-16) peuvent être utilisés
comme sorties directes spatialisées.

Dans l\'exemple suivant, la source 5 est envoyée directement au
haut-parleur 9 et la source 8 au haut-parleur 14. Les deux enceintes 9
et 14 restent dans la configuration DOME. Enfin, les sources 15-16 sont
envoyées aux sorties directes indépendantes 17-18 :

![](sources/media-fr/media/image78.png){width="4.57in"
height="5.7413024934383206in"}

NOTE: Comme les sorties directes sont affectées à des sorties
spécifiques, si vous ouvrez un projet avec un nombre de sorties directes
différent de celui du speaker setup que vous utilisez, certaines sorties
risquent d\'être coupées ! Il n\'y a pas d\'avertissement à ce sujet !

### 5.8.5. Show Speaker Numbers

L\'emplacement des haut-parleurs et leurs numéros peuvent être
visualisés dans la fenêtre 3D en choisissant l\'option Show Speaker
Numbers (Opt-Z). Les sorties directes sont affichées en noir. Un clic
sur un haut-parleur ou sur son numéro le sélectionne ; un clic droit le
désélectionne. Dans l\'image ci-dessus, le haut-parleur 3 est
sélectionné et les sorties directes indépendantes 17-18 sont en noir.
Show Speaker Numbers ne fonctionne que si l\'option Show Speakers est
activée dans le menu View.

## 5.9. Sources et Speakers

*SpatGRIS* reçoit les signaux audios du SAN et les envoie aux
haut-parleurs. Les deux sections principales sont les Sources (provenant
du SAN via *BlackHole*) et les Speakers. Il y a aussi les sorties
directes qui sont envoyées directement des sources vers ces
haut-parleurs (pour les subwoofers, par exemple).

![](sources/media-fr/media/image79.png){width="5.25in"
height="4.8819192913385825in"}

Dans cet exemple, les sources sont composées de 4 X sources
octophoniques (1-32), plus 1 X source stéréo (33-34), 1 X sorties
directes stéréo spatialisées (35-36 envoyées à 53-54) et 1 X sorties
directes indépendantes (37-38, assigné à 5-6) pour un total de 38
sources identifiées par différents groupes de couleurs, distribuées sur
un dôme de 32 haut-parleurs avec 2 sorties directes indépendantes (5-6).

### 5.9.1. Mute et Solo

Chaque source et chaque haut-parleur disposent d\'une touche Mute et
d\'une touche Solo.

![](sources/media-fr/media/image80.png){width="4.370860673665792in"
height="3.0in"}

### 5.9.2. Indicateurs de crête et réinitialisation

Un indicateur de crête est présent pour les Sources et les Speakers. Il
existe une fonction générale de Reset Meter Clipping dans le menu View
(Opt-M).

## 5.10. Les réductions stéréo

### 5.10.1. STEREO

Il existe un mode STEREO pour écouter un projet complexe sur une paire
de haut-parleurs. Tous les sons sont envoyés aux enceintes
correspondantes en fonction de leur emplacement (gauche à gauche, droite
à droite, pas d\'axe avant-arrière, pas d\'élévation). Lorsque STEREO
est sélectionné, l\'option de routage stéréo apparaît pour vous
permettre de choisir les sorties de votre choix, en fonction de votre
carte son. Seules les sorties de votre carte son sont disponibles pour
la réduction stéréo. En cas d\'utilisation de la carte de son interne de
l\'ordinateur, les sorties sont affectées aux numéros 1 et 2.

![](sources/media-fr/media/image81.jpg){width="2.385586176727909in"
height="0.8in"}

Ce mode peut être utilisé pour réduire un projet multicanal en stéréo.
Les sources sont simplement placées sur l\'axe Y, de gauche à droite.
Seul le Azimuth Span est utilisé en mode STEREO, et non pas le Elevation
span. Gardez à l\'esprit que les sources, à l\'exception des sorties
directes, ne sont jamais placées directement sur un haut-parleur, mais
sur plusieurs haut-parleurs --- au moins trois sur un DOME, beaucoup
plus sur un CUBE. Ainsi, la projection des sources n\'est probablement
pas aussi précise qu\'elle ne l\'est sur cette représentation !

![](sources/media-fr/media/image82.png){width="5.0in"
height="3.1433825459317584in"}

### 5.10.2. BINAURAL

Cet algorithme a été mis en œuvre pour aider les utilisateurs à
travailler sur la spatialisation 3D depuis leur maison lorsque l\'accès
à un dôme de haut-parleur est limité ou indisponible. Il est basé sur
une fonction de transfert liée à la tête (Head Related Transfer
Function, HRTF). La HRTF est une fonction qui reproduit la façon dont
nous percevons la localisation des sons dans l\'espace. Il s\'agit d\'un
ensemble de calculs de phase et d\'amplitude pour l\'écoute au casque.
Elle est principalement conçue pour les reproductions 5.1 ou l\'écoute
immersive au casque, situations que l\'on retrouve dans les jeux vidéo
et l\'industrie de la réalité virtuelle. Pour minimiser le nombre de
calculs (HRTF peut être très exigeant en termes de puissance de calcul),
*SpatGRIS* calcule d\'abord une spatialisation VBAP sur 16 haut-parleurs
(avec le BINAURAL_SPEAKER_SETUP, rendu invisible dans cette version) et
transfère ensuite le résultat à HRTF. Ne vous inquiétez pas, même si
votre configuration de haut-parleurs contient plus de 16 haut-parleurs,
aucune information n\'est perdue au cours du processus. Les modes
BINAURAL utilisent les sorties stéréo de votre choix. Les deux Spans
sont disponibles en mode BINAURAL.

Pour diverses raisons et à cause de considérations techniques, le niveau
sonore de sortie du mode STEREO diffère considérablement de celui du
mode BINAURAL, en fonction du nombre de sources. Veuillez ajuster votre
niveau d\'écoute en conséquence.

NOTE: Les Attenuation Settings utilisés en mode CUBE ou HYBRID sont
fonctionnels dans les réductions stéréo.

## 5.11. Enregistrement

Lorsque la composition de la spatialisation est terminée, deux options
s\'offrent à vous :

1\. Jouer le morceau \"en direct\" avec votre SAN et *SpatGRIS*.

2\. Enregistrer la spatialisation sur autant de pistes audios que le
nombre de haut-parleurs de la configuration.

*SpatGRIS* enregistre des fichiers mono (AIFF ou WAV selon vos
préférences) ou un fichier entrelacé.

Pour enregistrer : appuyez sur le gros bouton rouge en bas à droite de
la fenêtre principale.

![](sources/media-fr/media/image83.jpg){width="0.7916666666666666in"
height="0.7916666666666666in"}

Une fenêtre pop-up s\'ouvre alors, vous permettant de spécifier :

• L\'emplacement des fichiers enregistrés.

• Leur nom

• Le format : WAV ou AIFF.

• Le nombre de fichiers : Fichiers mono ou entrelacés.

• La possibilité d\'exporter le Speaker Setup pour la fonction Player
(chapitre 6).

Le fait d\'appuyer sur le bouton d\'enregistrement démarre
l\'enregistrement et la minuterie, et le bouton d\'enregistrement
devient clignotant. Une fois l\'enregistrement terminé, vous pouvez
appuyer à nouveau sur le bouton d\'enregistrement pour l\'arrêter. Vous
pouvez ensuite importer les fichiers monos séparés (ou un fichier
entrelacé) dans n\'importe quelle station de travail audionumérique pour
jouer votre morceau en concert.

![](sources/media-fr/media/image84.jpg){width="4.5in"
height="1.202884951881015in"}

Gardez à l\'esprit qu\'avec les fichiers entrelacés, il y a certaines
limites, et que ces limites sont atteintes assez rapidement sur les
grands projets :

\- AIFF est limité à 2 Go.

\- WAV est limité à 4 Go[^13].

De plus, si vous enregistrez un fichier entrelacé avec de nombreux
canaux, vous trouverez très peu de SAN capables de l\'ouvrir. Il est
donc préférable d\'enregistrer des fichiers monos.

# 6. PLAYER

*SpatGRIS,* à partir de la version 3.2, introduit un nouvel outil, le
PLAYER, qui permet d\'utiliser *SpatGRIS* comme logiciel autonome pour
jouer n\'importe quelle pièce enregistrée par *SpatGRIS* avec n\'importe
quelle configuration de haut-parleurs. L\'idée principale du PLAYER est
de faciliter la diffusion d\'œuvres multicanaux parmi différent.e.s
utilisateur.rice.s et sur différentes configurations de haut-parleurs.
Les œuvres réalisées avec un Speaker Setup DOME peuvent être jouées sur
un Speaker Setup CUBE et vice versa. Les sorties directes sont assignées
automatiquement, mais peuvent être ajustées manuellement par la suite.

## 6.1. Effectuer un enregistrement pour le PLAYER

La procédure d\'enregistrement d\'une pièce pour la reproduction avec le
PLAYER est presque identique à celle d\'un enregistrement normal. La
principale différence est que, en plus de l\'enregistrement des fichiers
audio eux-mêmes, vous devez exporter les coordonnées du Speaker Setup
utilisé en activant la fonction Export Speaker Setup. Les fichiers
audios et le Speaker Setup seront placés dans le même dossier et doivent
y rester pour que le PLAYER fonctionne correctement. Ces coordonnées
seront utilisées par le PLAYER pour positionner correctement les sources
dans n\'importe quel Speaker Setup.

![](sources/media-fr/media/image85.jpg){width="4.5in"
height="1.1701924759405073in"}

NOTE: Seuls les fichiers monos fonctionnent avec le PLAYER. Vous
obtiendrez un message d\'erreur si vous essayez d\'ouvrir un fichier
entrelacé. La raison en est que le PLAYER utilise les numéros des
sorties dans le nom des fichiers audio pour la spatialisation. Il n\'y a
aucun moyen d\'encoder cette information dans un fichier audio
entrelacé.

![](sources/media-fr/media/image86.jpg){width="1.4773589238845144in"
height="1.5in"}

## 6.2. Ouvrir et lire un projet avec le PLAYER

Une fois l\'enregistrement terminé, vous pouvez envoyer le dossier
contenant les fichiers sonores et le Speaker Setup à un.e auditeur.trice
qui utiliserait un autre dispositif de haut-parleurs. Vous pouvez aussi
l\'utiliser vous-même pour écouter l\'enregistrement sur un autre
dispositif de haut-parleurs.

### 6.2.1. Ouvrir le Speaker Setup pour l\'écoute

Ouvrir le Speaker Setup dans *SpatGRIS* sur lequel vous avez
l\'intention d\'écouter le travail spatialisé. Il peut s\'agir d\'une
configuration personnalisée ou d\'une configuration provenant des
Templates.

### 6.2.2. Ouvrir la fenêtre PLAYER et charger les fichiers

View Menu ---\> Show Player View

Load the audio files and Speaker Setup folder:

![](sources/media-fr/media/image87.jpg){width="5.5in"
height="2.928044619422572in"}

Le PLAYER affiche maintenant la forme d\'onde des fichiers audio :

![](sources/media-fr/media/image88.jpg){width="5.5in"
height="2.928044619422572in"}

Le PLAYER affiche également le dispositif de haut-parleurs avec lequel
l\'œuvre a été enregistrée. L\'emplacement des haut-parleurs d\'origine
est indiqué en rouge :

![](sources/media-fr/media/image89.jpg){width="4.714285870516186in"
height="3.0in"}

Veuillez noter que le projet actuel chargé dans *SpatGRIS* est remplacé
par le projet de l\'enregistrement.

### 6.2.3. Jouer la pièce

Le PLAYER est maintenant prêt à jouer la pièce. Il suffit d\'utiliser
les boutons Play et Stop. Il est également possible de cliquer
n\'importe où dans le fichier audio pour démarrer la lecture à partir de
cet endroit.

### 6.2.4. DOME dans CUBE ou CUBE dans DOME

Voici un exemple d\'enregistrement réalisé avec un dôme
(Dome20(8-6-4-2)Subs4) et joué dans un cube (Cube24(2X12)Subs2). Comme
on peut le voir, la forme du dôme original est bien reproduite dans le
cube d\'écoute :

![](sources/media-fr/media/image90.jpg){width="5.5in" height="3.0in"}

Voici un autre exemple montrant la situation inverse, un enregistrement
de cube (Cube24(3X8)Subs2) joué dans un dôme (Dome20(8-6-4-2)Subs4).
Comme on peut le voir, la forme du cube original est bien reproduite
dans le dôme d\'écoute :

![](sources/media-fr/media/image91.jpg){width="5.5in" height="3.0in"}

### 6.2.5. Les sorties directes dans le PLAYER

Le PLAYER essaiera d\'assigner les sorties directes originelles aux
sorties directes du dispositif d\'écoute.

Dans le premier exemple, la configuration d\'origine comportait quatre
sorties directes (numéros **6-12-18** et **24**). Mais dans la
configuration d\'écoute, il n\'y a que deux sorties directes (**25** et
**26**). Le PLAYER a assigné alternativement les numéros de sorties
directes originelles aux sorties directes disponibles dans la
configuration d\'écoute. Ces numéros de sortie peuvent être réglés
manuellement par la suite :

![](sources/media-fr/media/image92.jpg){width="5.5in"
height="2.878685476815398in"}

## 6.3. Sauvegarder un projet PLAYER

Si vous avez modifié un élément du projet PLAYER, vous pouvez le
sauvegarder en utilisant le bouton Save Player Project. Ce document sera
automatiquement placé dans le même dossier que les fichiers audios et la
configuration des enceintes. Le bouton File Saved ! (Fichier sauvegardé)
clignotera pendant un certain temps au cours du processus. Tous les
fichiers doivent rester dans le même dossier. La prochaine fois que vous
utiliserez le bouton Load audio files and Speaker Setup folder, tout
sera placé correctement en fonction de la façon dont il a été
sauvegardé.

![](sources/media-fr/media/image93.jpg){width="5.5in"
height="2.9427351268591426in"}

NOTE: Un projet du PLAYER reste actif tant que la fenêtre PLAYER est
ouverte. Lorsque vous la fermez, *SpatGRIS* passe à son mode d\'entrée
normal, attendant que l\'audio et l\'OSC proviennent d\'un séquenceur ou
de tout autre logiciel.

# 7. Menus

## 7.1. Menu File

Dans le menu File (Fichier), vous trouverez toutes les fonctions liées
au projet, où vous pourrez :

![](sources/media-fr/media/image94.jpg){width="1.6in"
height="1.5756944444444445in"}

![](sources/media-fr/media/image95.png){width="1.6in"
height="1.3590277777777777in"}![Immagine che contiene testo, schermata,
Carattere, numero Descrizione generata
automaticamente](sources/media-fr/media/image95.png){width="1.6in"
height="1.3590277777777777in"}• Créer un New Project.

• Ouvrir un projet existant.

• Ouvrir un projet à partir du dossier Project Templates. Ces modèles ne
peuvent pas être modifiés, mais ils peuvent être édités et enregistrés
en tant que nouveau fichier.

• Save Project or Save As --- pour faire une copie.

• Ouvrir un Speaker Setup.

• Ouvrir un Speaker Setup à partir du dossier Speaker Setup Templates.
Ces modèles ne peuvent pas être modifiés, mais ils peuvent être édités
et sauvegardés dans un nouveau fichier.

• Save Speaker Setup or Save As --- faire une copie.

• Ouvrir la fenêtre Settings.

## 7.2. Menu View

Dans le menu View, vous pouvez choisir différentes perspectives pour
visualiser les haut-parleurs et les sources en temps réel. La touche
modificatrice de ce menu est Option (Opt) pour Mac et Alt pour Windows.

![](sources/media-fr/media/image49.jpg){width="1.8in"
height="2.6868055555555554in"}![](sources/media-fr/media/image96.png){width="1.8in"
height="2.06292104111986in"}• Show 2D view : Une vue en 2D depuis le
haut du dispositif est affichée, montrant uniquement les sources.

• Speaker Setup Edition : Ouvre une fenêtre permettant d\'accéder à tous
les paramètres d\'une configuration de haut-parleurs.

•Show Player View: Ouvre la fenêtre du Player

• Show OSC monitor : Pour les spécialistes ! Pour aider à dépanner les
flux de messages OSC entrants.

• Show SpeakerView: Ouvre la fenêtre 3D des haut-parleurs

---

Keep Seaker View On Top

---

• Show Hall: Affiche les murs de la salle

• Show Numbers : Permet d\'afficher ou de masquer les numéros des
sources et/ou des enceintes affichées.

• Show Speakers : Permet d\'afficher ou de masquer les haut-parleurs
dans la vue 3D.

• Show Speakers Triplets : Affiche ou cache les triplets dans la vue 3D
en mode DOME. Il n\'y a pas de triplets en mode CUBE.

• Show Source Activity: Cette option permet de voir la position et les
trajectoires des sources (gros points) et leurs valeurs d\'azimut et
d\'élévation (petits points), selon les données envoyées par le
plugiciel *ControlGRIS2*. Notez qu\'il n\'y a rien à voir lorsque la SAN
est arrêtée. Le seuil est fixé à -70 dB. Lorsque cette option n\'est pas
sélectionnée, toutes les sources faisant partie d\'un projet sont
affichées, même lorsque la SAN est arrêtée. Cette option peut être utile
pour vérifier qu\'il n\'y a pas de canaux OSC en double envoyés par
*ControlGRIS2* vers *SpatGRIS*.

![](sources/media-fr/media/image97.jpg){width="2.1232086614173227in"
height="1.968503937007874in"}![](sources/media-fr/media/image98.jpg){width="2.1232086614173227in"
height="1.968503937007874in"}

  -----------------------------------------------------------------------
  *Show Source Activity* Off:       *Show Source Activity* On: Affiche
  Affiche la position de toutes les uniquement l\'activité réelle des
  sources                           sources en mode lecture
  --------------------------------- -------------------------------------

  -----------------------------------------------------------------------

• Show Speaker Level : Indique la quantité d\'énergie délivrée par
chaque haut-parleur. Du gris (rien) au blanc (maximum).

• Show Sphere/Cube : Si vous avez la possibilité de jouer dans une
sphère ou un cube complet !

---

• Colorize Sources : Cette option vous permet de régler toutes les
sources sur une couleur différente dans le spectre visible, du rouge au
violet. Attention, cette option efface toutes les couleurs
personnalisées déjà en place.

• Reset Sources Position: Lorsque vous passez d\'un projet à un autre,
*SpatGRIS* peut parfois afficher les sources du projet précédent.
Utilisez cette option pour effacer la vue 3D.

• Reset Meter Clipping: Les indicateurs de crête peuvent être
réinitialisés individuellement en cliquant dessus, ou globalement avec
le raccourci Opt-M.

## 7.3. Nommer et sauvegarder

*SpatGRIS* comporte trois composantes qui sont sauvegardées
indépendamment l\'une de l\'autre : Project, Speaker Setup and Settings.

• Save Project. Un projet est couplé à une œuvre.

• Save Speaker Setup. Un speaker setup est couplé à une installation
physique placée dans un espace.

• Save Settings. Ces paramètres sont liés à une station de travail
(ordinateur et interface audio), y compris les sorties stéréo utilisées
pour les réductions stéréo.

Speaker setups and Project documents sont enregistrés au format .xml. Il
n\'y a pas de distinction entre les deux. Le document de projet
n\'inclut pas le Speaker setup et ils sont donc indépendants. Par
conséquent, nous recommandons fortement deux choses :

• Ajoutez le mot \"Speaker Dome\" ou \"Speaker Cube\" au nom de vos
Speaker Setups et \"Project Dome\", \"Project Cube\" ou \"Project
Hybrid\" au nom de vos fichiers de projet.

• Enregistrez les Speaker Setup DOME ou CUBE dans deux dossiers
distincts dans un dossier nommé Speakers.

• Enregistrez les projets *SpatGRIS* dans trois dossiers distincts à
l\'intérieur d\'un dossier nommé Projects.

Les menus Templates que nous fournissons avec *SpatGRIS* sont un bon
exemple de la bonne classification.

• Avertissements concernant le format du document

*SpatGRIS* se souvient toujours du dernier speaker setup et du dernier
projet ouverts.

Si vous essayez d\'ouvrir un projet *SpatGRIS* avec la commande Load
Speaker Setup (ou l\'inverse), vous serez averti :

![](sources/media-fr/media/image99.jpg){width="2.752648731408574in"
height="1.1023622047244095in"}![](sources/media-fr/media/image100.jpg){width="2.75in"
height="1.1023622047244095in"}

NOTE : Les documents *SpatGRIS* adoptent un nouveau format et ne sont
pas rétrocompatibles avec les anciennes versions de *SpatGRIS*. En
essayant d\'ouvrir un projet *SpatGRIS* ou un dispositif de
haut-parleurs de la version 2, vous obtiendrez l\'un de ces messages
effrayants ! Vos fichiers sont corrects, mais ils ne sont pas
compatibles :

![](sources/media-fr/media/image101.jpg){width="2.75in"
height="1.1in"}![](sources/media-fr/media/image102.jpg){width="2.75in"
height="1.1in"}

## 7.4. Représentations

Les vues 3D et 2D de *SpatGRIS* sont disponibles pour les modes DOME et
CUBE. Dans le mode DOME, les sources se trouvent sur la surface et les
Spans s\'étendent le long de cette surface. En mode CUBE, les sources
peuvent être placées n\'importe où dans l\'espace et les Spans
s\'étendent localement autour des sources.

### 7.4.1. Représentation 3D

La fenêtre 3D en mode DOME (à gauche) ou en mode CUBE (à droite) de la
même session. Les haut-parleurs et les sources sont représentés :

![](sources/media-fr/media/image103.jpg){width="2.75in"
height="2.2998972003499563in"}![](sources/media-fr/media/image104.jpg){width="2.75in"
height="2.3028313648293963in"}

### 7.4.2. Représentation 2D 

La vue 2D en mode DOME (à gauche) ou en mode CUBE (à droite) de la même
session. Seules les sources sont représentées :

![](sources/media-fr/media/image105.jpg){width="2.3in"
height="2.3963243657042868in"}![](sources/media-fr/media/image106.jpg){width="2.3in"
height="2.396078302712161in"}

## 7.5. Performance et charge de travail du CPU

Les performances de la combinaison *ControlGRIS2/SpatGRIS* dépendent
largement des différents paramètres de votre projet. En règle générale,
un projet avec 64 canaux audios envoyés à 64 haut-parleurs fonctionnera
parfaitement bien sur des ordinateurs récents. Nous avons testé des
projets avec plus de 100 canaux audios sur une configuration de 128
haut-parleurs et cela fonctionnait toujours bien !

Les facteurs qui augmenteront de manière significative l\'utilisation du
CPU par nos outils sont, par ordre d\'importance:

• Le mode : CUBE est plus exigeant que DOME, car le premier utilise plus
de haut-parleurs que le second.

• Les Spans: Ils distribuent le signal à un plus grand nombre de
haut-parleurs que lorsqu\'ils ne sont pas utilisés, et la demande de CPU
augmente donc très rapidement à mesure que leurs valeurs augmentent.

• The Interpolation: le facteur d\'interpolation permet à certains sons
d\'obtenir une transition plus fluide lorsqu\'ils se déplacent d\'un
endroit à l\'autre. Par conséquent, plus ce paramètre est élevé, plus le
nombre de haut-parleurs impliqués dans le processus est important,
puisqu\'un son atteindra un haut-parleur donné plus tôt et mettra plus
de temps à le quitter (sans parler du fait que cela rend la localisation
plus floue).

• Le nombre de haut-parleurs utilisés dans *SpatGRIS*. Nous avons mesuré
des performances confortables avec une configuration de 96
haut-parleurs, ce qui est largement suffisant dans la plupart des
situations réalistes !

• Le nombre de pistes multiplié par le nombre de haut-parleurs détermine
la fiabilité de l\'installation. Peu de pistes sur un grand dispositif
donneront le même résultat que beaucoup de pistes sur un petit
dispositif.

Si le CPU dépasse les 100%, vous recevrez cette alerte :

![](sources/media-fr/media/image107.jpg){width="1.600479002624672in"
height="0.3937007874015748in"}

Vous voulez savoir à quoi vous attendre? Essayez vous-même !

## 7.6. Menu d\'aide

Le menu Aide comprend des informations sur le GRIS et sur ce manuel,
sous l\'option Open Documentation.

![](sources/media-fr/media/image12.jpg){width="1.8122222222222222in"
height="0.7in"}

**Sautez dans le vide et amusez-vous !**

# 8. Addendum

## 8.1. Descriptions des Sources Link 

### 8.1.1. Azimuth-Elevation et Azimuth-Distance

+-----------------------------------------------------------------------+
| **1) Independent** MONO + STEREO + MULTIPHONIQUE                      |
+=======================================================================+
| Ce mode est sélectionné par défaut. Les sources peuvent être          |
| déplacées indépendamment les unes des                                 |
| autres.!                                                              |
| [](sources/media-fr/media/image108.jpeg){width="1.3333333333333333in" |
| h                                                                     |
| eight="1.0in"}![](sources/media-fr/media/image109.jpeg){width="1.0in" |
| height="1.0in"}                                                       |
+-----------------------------------------------------------------------+
| **2) Circular** STEREO + MULTIPHONIQUE                                |
+-----------------------------------------------------------------------+
| !                                                                     |
| [](sources/media-fr/media/image110.jpeg){width="0.9528827646544182in" |
| height="1.0in"}Ce mode permet le mouvement circulaire groupé. Les     |
| angles entre les sources restent constants tandis que le rayon        |
| s\'ajuste                                                             |
| proportionnellement.!                                                 |
| [](sources/media-fr/media/image111.jpeg){width="0.9978816710411199in" |
| height="1.0in"}                                                       |
+-----------------------------------------------------------------------+
| **3) Circular Fixed Radius** STEREO + MULTIPHONIQUE                   |
+-----------------------------------------------------------------------+
| ![](sources/media-fr/media/image112.jpeg){width="1.046550743657043in" |
| height="1.0in"}!                                                      |
| [](sources/media-fr/media/image113.jpeg){width="0.9978816710411199in" |
| height="1.0in"}Les sources sont liées dans un mouvement circulaire    |
| par le paramètre Radius, qui reste fixe et égal. La distance relative |
| entre chaque source et le centre est la même pour toutes les sources. |
+-----------------------------------------------------------------------+
| **4) Circular Fixed Angle** STEREO + MULTIPHONIQUE                    |
+-----------------------------------------------------------------------+
| !                                                                     |
| [](sources/media-fr/media/image114.jpeg){width="0.8333333333333334in" |
| height="1.0in"}Les sources sont liées dans un mouvement circulaire    |
| avec le paramètre Angle, qui reste fixe et égal.                      |
|                                                                       |
| Par exemple, en octophonie, l\'angle d\'ouverture entre chacune des   |
| sources sera fixé à                                                   |
| 45°.![](sources/media-fr/media/image115.jpeg){width="1.0in"           |
| height="1.0in"}                                                       |
+-----------------------------------------------------------------------+
| **5) Circular Fully Fixed** STEREO + MULTIPHONIQUE                    |
+-----------------------------------------------------------------------+
| !                                                                     |
| [](sources/media-fr/media/image116.jpeg){width="1.0016699475065616in" |
| height="1.0in"}Les sources sont liées dans un mouvement circulaire    |
| par les paramètres Radius et Angle, qui restent fixes et égaux.       |
| L\'ouverture entre les sources et leur rayon est donc toujours        |
| identique. ![](sources/media-fr/media/image117.jpeg){width="1.0in"    |
| height="1.0in"}                                                       |
+-----------------------------------------------------------------------+
| **6) Delta Lock** STEREO + MULTIPHONIQUE                              |
+-----------------------------------------------------------------------+
| !                                                                     |
| [](sources/media-fr/media/image118.jpeg){width="1.2170384951881015in" |
| height="1.0in"}Ce mode verrouille la position des sources par rapport |
| aux autres selon les axes X et Y, sans possibilité de                 |
| rotation.![](sources/media-fr/media/image119.jpeg){width="1.0in"      |
| height="1.0in"}                                                       |
+-----------------------------------------------------------------------+

  ------------------------------------------------------------------------
  **7) Symmetric X** STEREO
  ------------------------------------------------------------------------
  ![](sources/media-fr/media/image120.jpeg){width="1.3333333333333333in"
  height="1.0in"}![](sources/media-fr/media/image121.jpeg){width="1.0in"
  height="1.0in"}Ce mode permet la symétrie entre deux sources suivant
  l\'axe X

  **8) Symmetric Y** STEREO

  ![](sources/media-fr/media/image122.jpeg){width="1.3333333333333333in"
  height="1.0in"}Ce mode permet la symétrie entre deux sources suivant
  l\'axe Y.![](sources/media-fr/media/image123.jpeg){width="1.0in"
  height="1.0in"}
  ------------------------------------------------------------------------

### 8.1.2. Elevation (Mode CUBE uniquement)

  -----------------------------------------------------------------------
  **1) Independent** MONO + STEREO + MULTIPHONIQUE
  -----------------------------------------------------------------------
  ![](sources/media-fr/media/image124.jpg){width="0.9465409011373578in"
  height="1.0in"}Ce mode est sélectionné par défaut. Les sources peuvent
  être déplacées indépendamment les unes des autres.

  **2) Fixed Elevation** STEREO + MULTIPHONIQUE

  ![](sources/media-fr/media/image125.jpg){width="0.9375in"
  height="1.0in"}Même élévation pour chaque source.

  **3) Bottom Top** STEREO + MULTIPHONIQUE

  ![](sources/media-fr/media/image126.jpeg){width="0.946428258967629in"
  height="1.0in"}Ce mode bloque la position des sources d\'une valeur
  minimale à une valeur maximale dans une relation linéaire.

  **4) Top Bottom** STEREO + MULTIPHONIQUE

  ![](sources/media-fr/media/image127.jpg){width="0.9402777777777778in"
  height="1.0in"}Ce mode verrouille la position des sources d\'une valeur
  maximale à une valeur minimale dans une relation linéaire.
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------
  **5) Delta Lock** STEREO + MULTIPHONIQUE
  -----------------------------------------------------------------------
  ![](sources/media-fr/media/image128.jpg){width="0.9465409011373578in"
  height="1.0in"}Ce mode verrouille la position des sources par rapport
  aux autres.

  -----------------------------------------------------------------------

## 8.2. Descriptions des trajectoires 

### 8.2.1. Azimuth-Elevation et Azimuth-Distance

+-----------------------------------------------------------------------+
| **1) Circle**                                                         |
+=======================================================================+
| ![](sources/media-fr/media/image129.jpg){width="0.9409722222222222in" |
| height="1.0in"}Mouvement circulaire autour du centre.                 |
|                                                                       |
| Options : CW/CCW (Sens horaire/ sens antihoraire), Back & Forth       |
| (va-et-vient), Dampening (amortissement), Deviation (déviation).      |
+-----------------------------------------------------------------------+
| **2) Ellipse**                                                        |
+-----------------------------------------------------------------------+
| ![](sources/media-fr/media/image130.jpg){width="0.94080927384077in"   |
| height="1.0in"}Mouvement elliptique autour du centre.                 |
|                                                                       |
| Options : CW/CCW (Sens horaire/ sens antihoraire), Back & Forth       |
| (va-et-vient), Dampening (amortissement), Deviation (déviation).      |
+-----------------------------------------------------------------------+
| **3) Spiral**                                                         |
+-----------------------------------------------------------------------+
| ![](sources/media-fr/media/image131.jpg){width="0.9404757217847769in" |
| height="1.0in"}Mouvement concentrique autour du centre.               |
|                                                                       |
| Options : CW/CCW (Sens horaire/ sens antihoraire), Back & Forth       |
| (va-et-vient), Dampening (amortissement), Deviation (déviation).      |
+-----------------------------------------------------------------------+
| **4) Square**                                                         |
+-----------------------------------------------------------------------+
| ![](sources/media-fr/media/image132.jpg){width="0.9439479440069991in" |
| height="1.0in"}Forme carrée autour du centre.                         |
|                                                                       |
| Options : CW/CCW (Sens horaire/ sens antihoraire), Back & Forth       |
| (va-et-vient), Dampening (amortissement), Deviation (déviation).      |
+-----------------------------------------------------------------------+
| **5) Triangle**                                                       |
+-----------------------------------------------------------------------+
| ![](sources/media-fr/media/image133.jpg){width="0.9409722222222222in" |
| height="1.0in"}Forme de triangle autour du centre.                    |
|                                                                       |
| Options : CW/CCW (Sens horaire/ sens antihoraire), Back & Forth       |
| (va-et-vient), Dampening (amortissement), Deviation (déviation).      |
+-----------------------------------------------------------------------+

### 8.2.2. Elevation (Mode CUBE uniquement)

+-----------------------------------------------------------------------+
| **1) Down Up**                                                        |
+=======================================================================+
| !                                                                     |
| [](sources/media-fr/media/image134.jpeg){width="0.9314643482064742in" |
| height="1.0in"} De bas en haut.                                       |
|                                                                       |
| Options : Back & Forth (va-et-vient) et Dampening (amortissement).    |
+-----------------------------------------------------------------------+
| **2) Up Down**                                                        |
+-----------------------------------------------------------------------+
| !                                                                     |
| [](sources/media-fr/media/image135.jpeg){width="0.9406255468066491in" |
| height="1.0in"} De haut en bas.                                       |
|                                                                       |
| Options: Back & Forth (va-et-vient) et Dampening (amortissement).     |
+-----------------------------------------------------------------------+

## 8.3. Messages OSC dans SpatGRIS

Les messages OSC peuvent être envoyés directement à *SpatGRIS* sans
avoir à utiliser *ControlGRIS2*.

Numéro du port d\'entrée de l\'OSC : 18032 par défaut (peut être modifié
dans File -\> Settings)

L\'adresse du serveur est toujours /spat/serv.

**Veuillez noter que les angles sont toujours mesurés dans le sens
horaire, en partant du centre de la scène (direction Y positive).**

**pol** déplace une source en utilisant des coordonnées polaires en
radians.

  -----------------------------------------------------------------------------
  **#parameter**   **type**   **valeurs            **signification**
                              autorisées**         
  ---------------- ---------- -------------------- ----------------------------
  1                string     pol                  \-

  2                int        \[1, 128\]           Source index

  3                float      any                  azimuth angle

  4                float      any                  elevation angle

  5                float      \[-3.0, 3.0\]        radius

  6                float      \[0, 1\]             Horizontal span

  7                float      \[0, 1\]             Vertical span
  -----------------------------------------------------------------------------

ex : Le message /spat/serv pol 7 0.0 0.78 0.5 0.1 0.2 déplace la source
n° 7 à l\'avant, à mi-hauteur et à la moitié de la distance de
l\'origine, avec un Span horizontal de 10 % et un Span vertical de 20 %.

**\
**

**deg** éplace une source en utilisant des coordonnées polaires en
degrés.

  ------------------------------------------------------------------------
  **index**      **type**   **valeurs          **signification**
                            autorisées**       
  -------------- ---------- ------------------ ---------------------------
  1              string     deg                \-

  2              int        \[1, 128\]         Source index

  3              float      any                azimuth angle

  4              float      any                elevation angle

  5              float      \[-3.0, 3.0\]      radius

  6              float      \[0, 1\]           Horizontal span

  7              float      \[0, 1\]           Vertical span
  ------------------------------------------------------------------------

ex : Le message /spat/serv deg 7 -90.0 45.0 0.5 0.1 0.2 déplace la
source #7 à l\'extrême gauche, à la moitié de l\'élévation et à la
moitié de la distance de l\'espace, avec un Span horizontal de 10% et un
Span vertical de 20%.

**car** déplace une source en utilisant des coordonnées cartésiennes.

  -------------------------------------------------------------------------
  **index**      **type**      **valeurs        **signification**
                               autorisées**     
  -------------- ------------- ---------------- ---------------------------
  1              string,       car              \-

  2              int           \[1, 128\]       Source index

  3              float         \[-1.66, 1.66\]  x (left/right)

  4              float         \[-1.66, 1.66\]  y (back/front)

  5              float         \[-1.66, 1.66\]  z (down/up)

  6              float         \[0, 1\]         Horizontal span

  7              float         \[0, 1\]         Vertical span
  -------------------------------------------------------------------------

ex : le message /spat/serv car 7 1.0 1.0 1.0 0.0 0.0 déplace la source
n° 7 dans le coin supérieur droit, sans Span horizontal ou vertical.

**clr** efface la position d\'une source.

  -------------------------------------------------------------------------
  **index**        **type**     **valeurs      **signification**
                                autorisées**   
  ---------------- ------------ -------------- ----------------------------
  1                string       clr            clear

  2                int          \[1, 128\]     Source index
  -------------------------------------------------------------------------

ex : Le message /spat/serv clr 7 efface la position de la septième
source.

**alg** sets a source\'s hybrid spatialization mode.

  -----------------------------------------------------------------------
  **index**         **type**   **valeurs        **signification**
                               autorisées**     
  ----------------- ---------- ---------------- -------------------------
  1                 string     alg              \-

  2                 int        \[1, 128\]       Source index

  3                 string     dome or cube     Algorithm
  -----------------------------------------------------------------------

ex : Le message /spat/serv alg 7 cube définit l\'algorithme de
spatialisation de la septième source sur \"cube\" (ne fonctionne qu\'en
mode hybride).

## 8.4. Messages OSC dans ControlGRIS2

Voici les messages OSC que *ControlGRIS2* peut envoyer et recevoir. Le
premier numéro correspond à l\'ID du plugiciel. Le second numéro
correspond au numéro de la source. Ce sont les valeurs par défaut :

• /controlgris/1/traj/1/x value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/y value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/z value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xyz/1 value =\> \[0.0;1.0\] 

• /controlgris/1/traj/1/xyz/2 value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xyz/3 value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xy values =\> \[0.0;1.0\] \[0.0;1.0\]

• /controlgris/1/traj/1/xyz values =\> \[0.0;1.0\] \[0.0;1.0\]
\[0.0;1.0\]

• /controlgris/1/azispan value =\> \[0.0;1.0\]

• /controlgris/1/elespan value =\> \[0.0;1.0\]

• /controlgris/1/sourcelink value =\> 1 to 8

1: Independent

2: Circular

3: Circular Fixed Radius

4: Circular Fixed angle

5: Circular Fully Fixed

6: Delta Lock

7: Symmetrix X

8: Symmetric Y

• /controlgris/1/sourcelinkalt value =\> 1 to 5

1: Independent

2: Equal Elevation

3: Bottom-Top

4: Top-Bottom

5: Delta Lock

• /controlgris/1/presets value =\> 1 to 50

• /controlgris/1/elevationmode value =\> 1 to 3

1: Normal

2: Extended Top

3: Extended Top and Bottom

## 8.5. Open Stage Control et Lemur

Deux contrôleurs externes sont disponibles pour *ControlGRIS* :

• Un patch pour Open Stage Control pour *iPad*™.

• Un patch pour Lemur pour *iPad*™.

Un manuel Addendum concernant ces patches est disponible sur
SourceForge.

## 8.6. Désinstaller

### 8.6.1. SpatGRIS

Si vous devez désinstaller *SpatGRIS*, ou si vous constatez un
comportement étrange du logiciel, vous devrez le faire manuellement.

• Mettez l\'application elle-même à la poubelle.

• Mettez ces fichiers à la poubelle :

\~/Bibliothèque/Preferences/ca.umontreal.musique.gris.spatgris.plist

\~/Application Support/GRIS/ SpatGRIS.x.x.xml où x.x.x représente la
version de *SpatGRIS* (3.2.11 par exemple).

### 8.6.2. ControlGRIS2

Si vous devez désinstaller *ControlGRIS2*.

Voici les parcours pour les utilisateur.trices de Mac :

• Pour désinstaller la version Audio Unit, supprimez-la de
l\'emplacement suivant :

\~/Bibliothèque/Audio/Plug-Ins/Components

• Pour désinstaller la version VST, supprimez-la du dossier VST à
l\'emplacement suivant :

\~/Bibliothèque/Audio/Plug-Ins/VST

• Pour désinstaller la version VST3, supprimez-la du dossier VST3 à
l\'emplacement suivant :

\~/Bibliothèque/Audio/Plug-Ins/VST3.

• Pour désinstaller la version AAX, supprimez-la à l\'emplacement
suivant :

MacIntosh HD/Bibliothèque/Application Support/Avid/Audio/Plug-Ins/

# 9. Problèmes connus et avertissements

Il y a tellement de situations et de configurations différentes qu\'il
nous serait impossible de les couvrir toutes. Jusqu\'à présent, nous
n\'avons trouvé aucune situation où le système ne fonctionne pas du
tout. Mais nous avons trouvé des situations où certains paramètres
doivent être ajustés avant que le système puisse fonctionner
correctement. En voici quelques-unes.

## 9.1. Problèmes connus

### 9.1.1. SpatGRIS, le plugiciel et SpatGRIS, le logiciel

Pour ceux qui ont utilisé le plugiciel *SpatGRIS*, vous remarquerez
qu\'il ne fonctionne plus sur les plus récents systèmes macOS et sur les
ordinateurs Apple Silicon. Nous recommandons de passer à *ControlGRIS2*.
Le développement de *SpatGRIS1* s\'est terminé en 2018.

### 9.1.2. 

### 9.1.3. 

## 9.2. Reaper 

### 9.2.1. Pistes mono 

• Créez une piste et insérez-y une instance de *ControlGRIS2* et un
fichier audio mono.

• Cliquez sur le bouton Route situé à droite du bouton de réglage du
gain de la piste.

• Dans la fenêtre qui s\'ouvre, décochez Master send.

• En bas à gauche de cette même fenêtre, cliquez sur le bouton Add new
hardware sortie\... (Ajouter une nouvelle sortie matérielle).

• Tout en bas de la liste des sorties de l\'interface de sortie se
trouvent les sorties individuelles mono.

• Sélectionnez la sortie qui correspond au numéro attribué à la source
dans *ControlGRIS2*.

Il n\'est pas nécessaire de panoramiser les sources monos vers la gauche
pour les pistes impaires et vers la droite pour les pistes paires,
puisque les sorties matérielles monos de Reaper sont utilisées. De plus,
la piste Master de Reaper est actuellement limitée à 128 canaux, il est
donc pratique d\'utiliser les sorties matérielles de Reaper directement
comme décrit.

### 9.2.2. Préférences avec Jack

Dans les Préférences de Reaper, sous l\'onglet Audio : décocher \"Close
audio device when stopped and application is inactive\". Sinon, *Jack*
perdra le contact avec Reaper lorsqu\'il est inactif, et le système ne
fonctionnera jamais.

![](sources/media-fr/media/image136.jpg){width="3.0in"
height="1.988830927384077in"}

## 9.3. Logic Pro

### 9.3.1. Une seule sortie Surround

Dans Logic Pro, il n\'y a qu\'une seule instance Surround possible. Cela
signifie qu\'il n\'est pas possible d\'avoir plusieurs pistes
multicanaux dans Logic tout en utilisant *SpatGRIS*. Pour éviter cette
restriction, n\'utilisez que des pistes mono et stéréo dans Logic.

### 9.3.2. Bouton Activate

Lorsque vous utilisez les trajectoires prédéfinies de *ControlGRIS2*, il
y a une exception concernant le bouton Activate dans Logic Pro. S\'il
n\'y a plus d\'audio dans la piste à la position d\'arrêt, le bouton
Activate ne s\'éteindra pas. Il devra être désactivé manuellement.

## 9.4. Digital Performer 11 et automatisation des mémoires

L\'automatisation des mémoires enregistrées dans DP présentent des
courbes lisses au lieu des courbes carrées attendues. Cela signifie que
le passage d\'une mémoire automatisée à une autre est progressif, alors
qu\'on s\'attend à ce qu\'il soit discret. Nous y travaillons.

## 9.5. Utilisation de SpatGRIS avec des entrées en direct

Dans le cas de l\'utilisation d\'entrées en direct, nous recommandons
l\'utilisation du périphérique agrégé sur un Mac. D\'après nos tests, le
système est stable lorsqu\'on crée un périphérique agrégé comprenant
*BlackHole* et la carte son que vous utilisez. Ce périphérique agrégé
doit être désigné comme périphérique d\'entrée et de sortie audio dans
votre SAN et comme périphérique d\'entrée et de sortie audio dans
SpatGRIS.

Pour la numérotation des canaux, veuillez vous référer à l\'application
Audio / Midi Configuration sur votre Mac une fois que vous avez créé
votre périphérique agrégé. En plaçant votre carte son physique comme
premier élément de périphérique, vous n\'aurez pas besoin de modifier la
numérotation des configurations de haut-parleurs. Ce flux de travail a
été testé avec Ableton Live.

Pour une utilisation sous Windows, l\'utilisation de Jack semble
suffisante, mais nous ne l\'avons pas testé de manière approfondie.

NOTE : Ajustez la taille de la mémoire tampon à la même valeur dans
votre SAN et dans *SpatGRIS*. Une valeur de 256 et plus est recommandée.

# 10. Conseil et astuces

Outre l\'usage normal de SpatGRIS qui permet de programmer la
spatialisation sonore de sources diverses et variées, voici quelques
exemples d\'usages différents, qui ne viennent pas à l\'esprit dans un
premier temps. C\'est avec les années que ces usages sont apparus à
travers les pratiques inventives de nos utilisateurs.

## 10.1. Spatialisation acousmatique

Il est tout à fait possible d\'utiliser SpatGRIS dans le cadre d\'une
spatialisation acousmatique traditionnelle, où une source stéréophonique
est multipliée sur autant de paires d\'enceintes dans la salle de
concert. Nous l\'avons utilisé de cette manière pendant des années lors
des concerts hebdomadaires du cours d\'Histoire de la musique électro.

### 10.1.1. Console de mixage

Pour arriver à faire de la spatialisation dans un contexte acousmatique,
il faut disposer d\'une console de mixage avec transmission Ethernet
(idéale, comme une AVID S1 ou une Euphonix) ou MIDI (plus lente, comme
une Mackie Control ou une Behringer).

### 10.1.2. Station Audio Numérique

Dans le SAN de votre choix (DP, Logic, Live, Nuendo, Reaper, etc.), vous
placez le fichier audio stéréo sur la première piste stéréo sur laquelle
vous placez également un plugiciel ControlGRIS2. Ensuite, vous
multipliez des copies de cette première piste stéréo sur autant
d\'exemplaires supplémentaires que comporte votre scénario de
spatialisation. Il est également possible de n\'avoir qu\'une seule
piste audio et autant de sorties auxiliaires que nécessaires, si votre
SAN le permet. Chaque piste et chaque instance de ControlGRIS2 seront
assignées à des numéros consécutifs. Il est important de mentionner ici
que l\'on n\'est pas dans une logique de correspondance un potentiomètre
= un haut-parleur. Chaque haut-parleur peut servir à plusieurs scénarios
de spatialisation.

### 10.1.3. Dispositif acousmatique

Utilisons le dispositif suivant Dome24(8-5x2-6)Subs2 Acousmonium présent
dans les Templates de SpatGRIS. Celui-ci est constitué de:

• 1 octophonie, de 1 à 8

• 1 paire asymétrique à gauche 9-10 (sorties directes)

• 1 paire solo centrale 11-12 (sorties directes)

• 1 paire stéréo principale 13-14 (sorties directes)

• 1 paire asymétrique à centre droit 15-16(sorties directes)

• 1 paire asymétrique à gauche 17-18(sorties directes)

• 1 groupe hexaphonique 19 à 24

• 1 paire de subwoofers 25-26 (sorties directes)

![](sources/media-fr/media/image137.jpg){width="3.136428258967629in"
height="2.8in"}

### 10.1.4. Scénario

Le premier scénario consisterait à assigner à chaque potentiomètre un
groupe de haut-parleurs dans l\'ordre mentionné ci-haut. Cela nécessite
8 potentiomètres, puisqu'il y a 8 groupes de haut-parleurs. Les sorties
directes n\'ont pas besoin de ControlGRIS2.

• Potentiomètre 1: ControlGRIS2 1-2, BlackHole sorties audio 1-2,
Position gauche-droite, Azimuth Span à 50%.

![](sources/media-fr/media/image138.jpg){width="1.6330938320209973in"
height="2.0in"}

Ainsi, la source stéréo est entièrement répartie sur les 8 hp du groupe
octophonique.

Le canal gauche sur les hp impairs (en turquoise pâle) et le canal droit
sur les hp pairs (en turquoise plus foncé):

![](sources/media-fr/media/image139.jpg){width="3.803847331583552in"
height="3.0in"}

• Potentiomètre 2: pas de ControlGRIS2, BlackHole sorties 3-4, H-P 9-10
sorties directes dans SpatGRIS (en noir):

![](sources/media-fr/media/image140.jpg){width="0.9209930008748907in"
height="2.0in"}![](sources/media-fr/media/image141.jpg){width="2.95918416447944in"
height="2.0in"}

• Potentiomètre 3: pas de ControlGRIS2, BlackHole sorties 5-6, H-P 11-12
sorties directes dans SpatGRIS (en noir):

![](sources/media-fr/media/image142.jpg){width="0.8968613298337708in"
height="2.0in"}![](sources/media-fr/media/image143.jpg){width="2.7224671916010497in"
height="2.0in"}

• Potentiomètre 4: pas de ControlGRIS2, BlackHole sorties 7-8, H-P 13-14
sorties directes dans SpatGRIS (en noir):

Même scénario

• Potentiomètre 5: pas de ControlGRIS2, BlackHole sorties 9-10, H-P
15-16 sorties directes dans SpatGRIS (en noir):

Même scénario

• Potentiomètre 6: pas de ControlGRIS2, BlackHole sorties 11-12, H-P
17-18 sorties directes dans SpatGRIS (en noir):

Même scénario

• Potentiomètre 7: ControlGRIS2 13-14, BlackHole sorties 13-14, H-P
19-24 Position gauche-droite, Azimuth Span à 50%, Élévation dans le haut
du dôme:

![](sources/media-fr/media/image144.jpg){width="1.940323709536308in"
height="1.8in"}![](sources/media-fr/media/image145.jpg){width="1.2369860017497813in"
height="1.8in"}

Le canal gauche sur les hp impairs (en orange pâle) et le canal droit
sur les hp pairs (en orange plus foncé):

![](sources/media-fr/media/image146.jpg){width="3.6548228346456693in"
height="2.0in"}

## 10.2. Utilisation du PLAYER en votre absence

Le PLAYER (voir le chapitre 6. PLAYER) est un outil très puissant dans
*SpatGRIS* qui permet d\'enregistrer un projet dans le dispositif
originel et ensuite de le jouer dans un autre dispositif, celui d\'une
salle de concert par exemple. La situation typique est celle où une de
vos œuvres est jouée ailleurs en votre absence. Vous pouvez alors
enregistrer votre projet grâce à la fonction Record (voir le chapitre
5.11. Enregistrement) en cochant la case Export Speaker Setup:

![](sources/media-fr/media/image85.jpg){width="4.5in"
height="1.1701913823272092in"}

Les fichiers audios et le dispositif de haut-parleurs originel seront
sauvegardés dans le même dossier. Vous pouvez faire parvenir celui-ci à
votre destinataire qui pourrait jouer votre pièce dans son propre
dispositif. Cette fonction est très utile pour contribuer à la diffusion
des musiques multicanales.

## 10.3. Le mode HYBRID pour varier les trajectoires

Le mode HYBRID (voir le chapitre 5.7. Le mode HYBRID) est en réalité un
DOME dans lequel il est possible de déplacer des sources en mode CUBE.
En mode DOME exclusif, les sources sont obligatoirement placées sur la
surface du dôme. C\'est l\'algorithme VBAP qui impose cela. Il n\'est
donc pas possible de placer un son à l\'intérieur du dôme ou à
l\'extérieur de celui-ci. En adoptant le mode HYBRID, les sources
peuvent soit se comporter en mode DOME, soit en mode CUBE:

![](sources/media-fr/media/image147.jpg){width="4.403225065616798in"
height="0.9in"}

Comme on peut le voir ici, certaines sources (en bourgogne) sont situées
à l\'extérieur du dôme alors que d\'autre (en bleu clair) sont à
l\'intérieur de celui-ci.

Le mode HYBRID permet ainsi de varier les trajectoires en mode DOME:

![](sources/media-fr/media/image148.jpg){width="6.5in"
height="4.235416666666667in"}

# Index

2

256 entrées et sorties · 8

3

3D et 2D · 52

A

Activate · 26

adresse du serveur · 57

AIFF est limité à 2 Go · 44

AIFF ou WAV · 43

Alt for Windows · 50

Apple Silicon M1-M2 · 8, 10

Attenuation (dB): · 35

Avertissements concernant le format du document · 52

Azimuth-Distance et Elevation · 20

Azimuth-Elevation · 19

B

Back & Forth · 24

BINAURAL · 43

*BlackHole* · 8

bouton d\'enregistrement · 44

C

canaux OSC · 19

cartésiennes (CUBE) · 18

Catalina · 10

conditions minimales · 38

crête · 42

CUBE · 16

D

dampening · 24

Descriptions des trajectoires · 56

désinstaller *ControlGRIS* · 59

désinstaller *SpatGRIS* · 59

Deviation · 24

DOME · 16

DP · 10

Drawing · 25, 26

E

Extended Top · 21

Extended Top et Bottom · 21

F

Filtrage (Hz) · 35

First Source ID · 17

format .xml · 51

G

Gaël Lane Lépine · 17

Global Sound Diffusion · 37

H

Head Related Transfer Function, HRTF · 43

HYBRID · 32

I

Interpolation · 53

IP Address · 17

J

*Jack* · 8

L

Le seuil est fixé à -70 dB · 50

Lemur · 19, 59

Live · 10

Logic Pro · 10

M

Maj-Clic en mode Drawing · 25

Matrix Base Amplitude Panning · 32

MBAP · 17

mémoire tampon · 11, 31

microphone · 9

multiclient · 13

Mute et Solo · 42

N

niveau de sortie de *SpatGRIS* · 13

Numéro du port d\'entrée de l\'OSC · 57

O

*OctoGris* · 10

onglet Sources · 18

Open Sound Control · 18

Open Stage Control · 8, 19, 59

Option (Opt) pour Mac · 50

Ordre des haut-parleurs · 37

OSC Input Port · 31

P

pendule · 26

performances · 53

polaires (DOME) · 18

presets automatisés · 27

R

Reaper · 10

*ReaRoute* · 8

Reset Meter Clipping · 51

Reset Sources Position · 51

S

Samuel Béland · 39

Save Project · 28

Save Settings · 28

Save Speaker Setup · 28

Sécurité et confidentialité · 9

Show Speaker Numbers · 40

Show Speaker Triplets · 32

Sorties directes indépendantes · 39

Sorties directes spatialisées · 39

Sources Link descriptions · 54

Spans · 20, 53

*SpatGris1* · 10, 60

*SpeakerView* · 29

STEREO · 42

subwoofers · 39

T

tempo MIDI · 24

trajectoires automatisées · 27

U

utilisation du CPU · 53

V

VBAP · 17

Vector Base Amplitude Panning · 32

Ville Pulkki. · 17

Volume (dB) · 35

W

WAV est limité à 4 Go · 44

Z

*ZirkOSC* · 10

[^1]: *BlackHole* n\'est pas obligatoire. Tout logiciel capable
    d\'envoyer de l\'audio à *SpatGRIS* peut être utilisé. *BlackHole*
    est un plugiciel HAL.

[^2]: Voir le format des messages OSC dans l\'addendum..

[^3]: JackRouter est un plugiciel HAL qui n\'était pas compatible avec
    MacOS 10.15 et plus, et qui n\'a pas été supporté pendant un certain
    temps.

[^4]: Conçu par Christophe Lengelé.

[^5]: Pour plus d\'informations, voir le lien suivant :
    https://jackaudio.org/downloads/

[^6]: Open Sound Control

[^7]: Nous n\'avons que peu testé sur Windows 11.

[^8]: Le plugiciel AAX pour Windows est signé à l\'aide d\'un certificat
    auto-émis. Il n\'est pas clair pour l\'instant si cela est suffisant
    pour ProTools et/ou Windows Defender.

[^9]: Depuis la version 3.2.0, le LBAP, Layer Base Amplitude Panning,
    conçu par Olivier Bélanger, n\'est plus utilisé.

[^10]: <http://opensoundcontrol.org>

[^11]: Voir le manuel Addendum pour plus d\'informations

[^12]: Sur Mac, la plupart des claviers utilisent Option (Opt), tandis
    que d\'autres utilisent Alt. Dans ce manuel, c\'est la touche Opt
    qui sera utilisée.

[^13]: Les formats CAF (Core Audio Format) et WAV RF64 seront
    éventuellement mis en œuvre, ce qui permettra de dépasser les 4 Go.
