# Simulateur de cold call (claude.ai, mode vocal)

Un kit qui transforme Claude en **prospect réaliste** et en **coach**, pour apprendre la prospection téléphonique à froid, même sans avoir jamais passé un seul appel.

Tout se passe dans claude.ai, en mode vocal : pas d'appli, pas de clé API, rien à payer en plus de ton abonnement. Les conversations vocales comptent simplement dans tes limites d'usage habituelles.

## Ce que contient le kit
```
simulateur-cold-call/
├── README.md                    ← ce mode d'emploi
├── instructions-projet.md       ← le texte court à coller dans « Instructions du projet »
└── connaissances/               ← les 8 fichiers à importer dans le projet
    ├── regles-du-simulateur.md  ← toutes les règles du prospect et du coach
    ├── mon-offre.md             ← ce que tu vends et à qui (déjà remplie : sites web pour artisans)
    ├── parcours.md              ← les 6 étapes pour progresser
    ├── methode.md               ← les bases que le coach t'enseigne (version artisans)
    ├── prospects.md             ← les 10 profils de prospects et les 3 barrages (secret)
    ├── variantes.md             ← humeurs, cartes secrètes, niveaux (secret)
    ├── objections.md            ← les objections et les façons d'y répondre
    └── grille-debrief.md        ← la notation et les débriefs
```

## Pourquoi Claude ne sera pas complaisant
- **Des prospects tirés au sort.** 10 profils × 10 humeurs × 10 cartes secrètes, soit 1 000 combinaisons. Chaque prospect a un **objectif caché** (raccrocher vite, obtenir un prix, se débarrasser de toi poliment…) et une **douleur cachée** qu'il ne révèle que si tu poses la bonne question.
- **Une jauge d'intérêt secrète.** Elle monte ou descend après chacune de tes phrases, selon des règles précises. Le prospect n'accepte un rendez-vous que si la jauge atteint un seuil, que tu as bien traité ses objections et que tu proposes un créneau précis.
- **Un coach exigeant et pédagogue.** Il t'apprend les bases, te fait monter par étapes et cite tes phrases. Il te propose aussi **plusieurs façons de répondre, chacune avec son objectif**.

## Installation (5 minutes)
1. Sur claude.ai, ouvre **Projets**, puis **Créer un projet**, et nomme-le « Simulateur cold call ».
2. Dans **Instructions du projet**, colle le texte de `instructions-projet.md`. Il est court exprès : un long texte collé peut être coupé sans prévenir.
3. **Importe les 8 fichiers** du dossier `connaissances/` dans les **connaissances du projet**. Importe les fichiers eux-mêmes, sans recopier leur contenu à la main.
4. `mon-offre.md` est déjà remplie pour la vente de sites web aux artisans. Si tu vends autre chose, remplace chaque champ par ta réponse (il y a un autre exemple rempli plus bas).
5. Dans **Réglages → Général → Voix → Langue**, choisis **Français**.
6. Choisis le modèle **Opus** (le plus fidèle au rôle) ou **Sonnet** (plus rapide, et il consomme moins tes limites). Évite Haiku : il tient moins bien un rôle exigeant.
7. **Vérifie l'installation.** Ouvre une nouvelle conversation dans le projet et écris « Vérifie l'installation ». Claude doit voir les 8 fichiers et confirmer que `regles-du-simulateur.md` se termine par la ligne « Fin des règles du simulateur. ». Si un fichier manque ou est coupé, supprime-le du projet et réimporte-le.

> Pour garder la surprise, ne lis pas `prospects.md` ni `variantes.md` : ce sont les fiches secrètes des prospects.

## Par où commencer (tu n'as jamais fait de cold call)
1. **Première séance, à l'écrit.** Ouvre une nouvelle conversation dans le projet et écris « Première séance ». En 20 à 30 minutes, le coach :
   - t'explique comment se déroule un appel ;
   - écrit ta trame d'appel avec toi (garde-la : tu peux l'ajouter au projet sous le nom `ma-trame.md`) ;
   - te fait une démo inversée, où il joue le commercial et toi le prospect.
2. **Ton premier appel.** Passe en vocal (l'icône en forme d'onde sonore) et dis « Nouvel appel, étape 1, mode guidé ».
3. **Ensuite, une séance de 15 à 20 minutes par jour**, dans une nouvelle conversation à chaque fois :
   - un échauffement (2 accroches ou 3 objections) ;
   - 2 à 3 appels de ton étape ;
   - « Coach, bilan ».

## Le parcours en 6 étapes
| Étape | Tu travailles | Pour passer à la suite |
|---|---|---|
| 1 | L'accroche (les 30 premières secondes) | 3 accroches réussies de suite, sur 3 profils différents, dont une au niveau 2 |
| 2 | La découverte | Les 3 informations clés obtenues sans monologue, sur 2 appels parmi 3 |
| 3 | Les objections | Au moins 3/5 de moyenne, sur deux séries d'entraînement de suite |
| 4 | L'appel complet (niveaux 1 et 2) | Rendez-vous avec au moins 60/100, deux appels de suite, dont le second au niveau 2 |
| 5 | Le barrage secrétaire, au niveau 3 | Barrage passé 2 fois sur 3, et 65/100 de moyenne |
| 6 | Les niveaux 4 et 5, avec des codes au hasard | 70/100 de moyenne : tu es autonome |

Dès l'étape 4, tu peux commencer de vrais appels. Le simulateur te sert alors d'échauffement, et à rejouer les appels difficiles.

## Les commandes
Pendant un appel, les commandes commencent par **« Coach »**. Tout le reste est ce que tu dis au prospect.

| Tu dis | Ce qui se passe |
|---|---|
| « Vérifie l'installation » | Claude vérifie que les 8 fichiers sont là et complets |
| « Première séance » | Accueil guidé : les bases, ta trame, une démo |
| « Nouvel appel, étape 2 » | Le coach choisit un prospect adapté à ton étape. Le prospect décroche. |
| « Nouvel appel, code 4-7-2, niveau 3 » | Prospect tiré au sort par le code, au niveau choisi |
| … « mode guidé » | Le coach glisse un conseil d'une phrase après une grosse erreur |
| … « avec barrage » | Le standard ou l'assistante décroche d'abord |
| … « objectif qualification » (ou accroche, barrage, rappel) | Change le but de l'appel (par défaut : décrocher un rendez-vous) |
| « Coach, joker » | Un conseil quand tu bloques (−5 points) |
| « Coach, stop » | Fin de l'appel et débrief court |
| « Débrief » / « Débrief complet » | Après l'appel : la version orale courte, ou la version écrite détaillée |
| « Coach, démo » | Démo inversée : Claude joue le commercial, toi le prospect |
| « Coach, leçon » | Une explication de 2 minutes sur ton étape |
| « Entraînement objections » | 5 objections à la suite, chacune notée sur 5 |
| « On rejoue » | Le même prospect, au même niveau |
| « Coach, plus dur » / « Coach, plus facile » | Change le niveau pour la suite |
| « Coach, bilan » | Le bilan de la séance |
| « Coach, voici mon journal » + tes lignes | La séance du jour, construite à partir de ton historique |

Hors appel, tu peux parler librement au coach. Par exemple, raconte-lui un vrai appel qui s'est mal passé et demande-lui de le rejouer avec toi.

## Pendant l'appel
- **Parle comme au vrai téléphone :** le prospect ne sait rien de toi et ne t'attendait pas.
- **Mode mains libres** (par défaut) : Claude répond dès que tu marques une pause, comme un prospect qui te coupe. Si ça te gêne, passe en **appui pour parler** : tu maintiens le bouton pendant que tu parles.
- **Les codes :** dis les chiffres séparément (« code 4, 7, 2 »). Pour un vrai hasard, prends les 3 derniers chiffres d'un numéro de téléphone ou d'une plaque d'immatriculation.
- **Les niveaux :** de 1 (débutant) à 5 (expert). Sans précision, c'est ton étape en cours qui décide.

## Après l'appel
- **Le débrief court** se fait à l'oral, après la question « Comment tu l'as senti, sur 10 ? ».
- **Le débrief complet :** arrête le mode vocal et tape « Débrief complet ». La conversation vocale est gardée en texte dans la conversation.
- **Ton journal :** chaque débrief se termine par une ligne de journal. Copie-la dans une note sur ton téléphone. En début de séance, dis « Coach, voici mon journal » et colle tes 5 dernières lignes.

## Dépannage
| Problème | Solution |
|---|---|
| Claude dit qu'un fichier manque, ou ne connaît pas une règle (mode guidé, commandes…) | Écris « Vérifie l'installation », puis réimporte le fichier manquant ou coupé. |
| Le prospect est trop gentil ou accepte trop vite | « Coach, plus dur ». Vérifie que tu es sur Opus ou Sonnet. Ouvre une nouvelle conversation. |
| Il sort du personnage ou commente l'appel | « Reste dans le personnage. » |
| Il lit des astérisques ou des didascalies | « Rappel : tout ce que tu écris est lu à voix haute, pas de didascalies. » |
| Il te coupe trop vite | Passe en appui pour parler. |
| Il ne réagit pas à une commande | Redis-la lentement, ou tape-la. |
| Il mélange les appels ou oublie des règles | La conversation est trop longue : ouvre-en une nouvelle à chaque séance. |
| Le mode vocal ne semble pas suivre le projet | Utilise le plan B ci-dessous. |

## Plan B : sans projet
1. Ouvre une conversation normale, hors projet.
2. Joins les 8 fichiers de `connaissances/`.
3. Colle le texte de `instructions-projet.md`, puis ajoute : « Confirme en une phrase, puis attends ma commande. »
4. Passe en vocal.

## Un autre exemple de fiche « mon offre »
Pour une offre différente (exemple inventé, chiffres compris) :
- Mon prénom et le nom que j'annonce au téléphone : Lucas, de RDV Facile
- En une phrase : un logiciel de prise de rendez-vous en ligne pour les cabinets de kinésithérapie
- Le problème que ça résout : le secrétariat passe des heures au téléphone, et les rendez-vous non honorés font perdre de l'argent
- Résultats ou preuves : 30 % de rendez-vous non honorés en moins grâce aux rappels par SMS, chez nos 40 cabinets clients
- Prix ou fourchette : 49 € par mois et par praticien
- Type d'entreprise : cabinets de 2 à 10 kinés, en Île-de-France
- La personne que j'appelle : le kiné titulaire, ou l'associé gérant
- Ce qu'ils font aujourd'hui : agenda papier ou vieux logiciel, et une secrétaire au téléphone
- Objectif d'un appel : une démo de 20 minutes en visio
- Mon accroche actuelle : [facultatif]
- Les objections que je redoute : « On a déjà un logiciel », « On n'a pas le temps de changer »

## Personnaliser
- **Les règles du prospect et du coach :** `regles-du-simulateur.md`.
- **Ajouter tes propres objections :** complète `objections.md` avec les phrases que tu entends en vrai.
- **Changer la difficulté :** les seuils et les jauges de départ sont dans le tableau des niveaux de `variantes.md`.
- **Ajouter un profil de prospect :** copie la structure d'un profil de `prospects.md`.
