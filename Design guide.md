NORMA LMI Blue - Design Guide


# 1 Introduction
Ce que couvre le présent rapport et qui en est responsable.
## 1.1 A propos de ce rapport
Ce rapport traite des motivations, de la philosophie, de l'utilisation et des intentions du modèle NORMA appliqué de lutte contre la désinformation.
Il fait partie d'une série de rapports sur la manière dont les principes et les pratiques de juridique peuvent être utilisés pour améliorer notre compréhension de la sécurité cognitive et améliorer les réponses aux opérations d'information, et plus particulièrement aux campagnes et incidents de désinformation.

## 1.2 Structure du présent rapport
Le présent rapport s'articule autour de sections sur la conception et l'utilisation d'e NORMA LMI blue , et peut être résumé comme suit :
- Cette section d'introduction : histoire de la création de NORMA LMI blue
- Conception et philosophie de NORMA LMI blue: pourquoi et comment nous avons construit les cadres, et les choix de conception que nous avons faits
- Conceptions des composants de NORMA LMI blue
- Utilisation de NORMA LMI Blue : outils, technique et utilisations suggérées
- Travaux futurs : notes et idées pour améliorer ce travail

Ce document accompagne le rapport les instruments juridiques dans la lutte contre les manipulations de l'information et la copie principale des modèles NORMA LMI Blue, contenus dans le dépôt github : https://github.com/NormaProject/LMI-Framework/

Ce rapport est un document évolutif. Il s'agit de la version 1.0.

## 1.3 Lutte contre les manipulations de l'information
Les acteurs étatiques, et les opérateurs d'influence privés exploitent l'ouverture et la portée de l'internet pour manipuler les populations à distance. Il s'agit d'une extension de la lutte pour les « cœurs et les esprits » menée depuis des décennies par le biais de la propagande, des opérations d'influence et de la guerre de l'information. 
Parmi les avancées récentes, on peut citer la propagande informatique : l'utilisation d'algorithmes, y compris l'apprentissage automatique et l'intelligence artificielle, dans la manipulation en ligne.
Il existe de nombreuses définitions de la désinformation, de la mésinformation, de l'incident, etc. et des équipes se consacrent à l'amélioration de ces définitions Le présent rapport utilise ces définitions de travail :
- La désinformation est la promotion délibérée d'informations fausses, trompeuses ou mal attribuées, généralement conçues pour modifier les croyances ou les actions d'un grand nombre de personnes, en tant qu'outil permettant d'atteindre un objectif extérieur.
- La mésinformation est une information fausse ou trompeuse qui est potentiellement nuisible. La structure et les modes de propagation des attaques de désinformation présentent de nombreuses similitudes avec celles observées dans le domaine de la sécurité de l'information et du piratage informatique.

Ces similitudes sont documentées dans le Framework DISARM offrant un panorama détaillé des comportements rencontrés.
 
En analysant et en exploitant les similitudes avec les cadres de sécurité de l'information, les défenseurs disposent de meilleurs moyens pour décrire, 
identifier et contrer les attaques basées sur les manipulations de l'informations (LMI).

Parmi les contres mesures identifiées par le Framework DISARM, quelques unes traitaient de moyens juridique. Nous avons choisit d'étendre les réflexions sur ce sujets en développant NORMA LMI Blue. 

## 1.4 NORMA et NORMA LMI Blue
NORMA est un ensemble de normes de données et une base de connaissances à source ouverte recensant les tactiques, techniques  et procédures composant les opérations juridiques de l'équipe rouge et de l'équipe bleue.

Il s’adresse aux professionnels du droit.

Son objectif est de leur donner la capacité de répondre tactiquement aux lawfare, de planifier des défenses et des contre-mesures, et de transférer les principes de sécurité de l'information aux opérations juridiques . 

Il fournit une taxonomie commune pour les opérations juridiques, un cadre pour partager rapidement les renseignements sur les menaces et un outil conceptuel pour renforcer les défenses par le biais d'une équipe rouge, d'une analyse des risques, de rediffusions et de simulations.

NORMA se compose de modèles d'équipe bleue (défense) et d'équipe rouge (attaque), ainsi que d'un référentiel de descriptions, d'atténuations et d'exemples.

NORMA LMI Blue détaille les opérations juridiques envisageables dans le cadre de la lutte contre les manipulation de l'information. 

Pour créer NORMA LMI Blue, nous avons placé les composants des opérations juridiques de lutte contre les manipulations de l'information dans un cadre basé sur les frameworks de référence(notamment DISARM, ATT&CK et STIX) couramment utilisées pour décrire les incidents liés à la sécurité de l'information.

 Le framework NORMA LMI blue  est conçu pour s'adapter aux mêmes ensembles d'outils et aux mêmes cas d'utilisation que DISARM STIX et ATT&CK.


## 1.5 Remerciements

# 2 Conception et philosophie de l'ensemble d'outils NORMA

L'ensemble d'outils NORMA est né de la nécessité de disposer d'un langage commun pour les opérations juridiques.

Au moment de sa création, notre communauté comprenait des universitaires, des professionnels de droit et de l’intelligence économique, des designers, des représentants d’associations professionnelles et des personnes d'autres disciplines qui avaient tous des mots différents pour désigner les concepts et les objets des opérations juridiques. 

Les outils NORMA devraient idéalement permettre à des personnes issues de différents domaines de parler d’opération juridique sans confusion.

Cette section explique pourquoi et comment nous avons construit le Framework NORMA LMI Blue, comment ses modèles sont reliés les uns aux autres et les choix de conception que nous avons faits lors de leur création.

## 2.1 Les manipulations de l'information en tant qu'écosystème

## 2.2 Mettre en relation les acteurs de la défense
Lorsque nous avons commencé, nous savions que notre meilleure chance de créer de bonnes défenses contre la désinformation impliquait de mettre en relation des personnes issues de mondes très différents :
- Les spécialistes des opérations d'information, expert en intelligence économique ou en opérations psychologiques, analysant les rapports de force et l'instrumentalisation des flux informationnels.
- Les scientifiques des données, qui analysaient des ensembles d'objets et des flux d'informations sur internet en utilisant des techniques telles que l'apprentissage automatique et l'analyse des réseaux sociaux pour démêler les modèles de comptes, de textes, de hashtags, d'urls, de groupes, et les relations entre eux tous.
- Les spécialistes des sciences sociales et les psychologues qui ont étudié les vulnérabilités cognitives humaines, la dynamique de groupe, ainsi que le flux et l'effet des récits sur les croyances et les émotions.
- Les experts en sécurité de l'information (infosec), qui avaient déjà construit des outils, des techniques et des processus pour protéger les informations détenues dans des topologies très similaires, qui au lieu d'être des communautés de personnes étaient des réseaux de machines.
- Les professionnels du droit, qui de part leur pratiques du droit des affaires, du contentieux ou/des arcanes de la procédure disposent d'une connaissance fine des instruments mobilisables un fois le fait juridique qualifié. 

## 2.3 Modèles d'opérations juridiques basés sur les composants

Il est utile de considérer une opération juridique ou une manipulation de l'information comme un ensemble d'objets et de relations entre eux. 

De nombreux chercheurs en désinformation organisent déjà leurs informations de cette manière (tout comme les recherches inspirées de l'OSINT, du renseignement et du journalisme sur lesquelles repose une grande partie de ce travail), certains de nos premiers collaborateurs allant même jusqu'à construire des « murs du meurtre » pour suivre les groupes et les incidents.

Ces modèles sont formalisés en tant que modèles de systèmes sociotechniques, c'est-à-dire des modèles de réseaux complexes de communautés, de comptes et de technologies en interaction qui constituent une opération juridique, un incident ou une campagne de manipulation de l'information.

Les communautés de l'infosec et de lutte contre les manipulation disposent déjà d'une norme de données à cet effet, STIX https://oasis-open.github.io/cti-documentation/, qui s'accompagne également d'une norme, TAXII, sur la manière de partager les données STIX entre les systèmes. 

Le projet NORMA développe une version de STIX pour les opérations juridiques, en adaptant ses types d'objets existants à la manipulation de l'information. 

Il existe d'autres modèles de désinformation basés sur les composants, notamment le modèle ABC  “Actor, Behaviour, Content” « Acteur, Comportement, Contenu » de Camille François et son extension, ABCDE (« Acteur, Comportement, Contenu, Degré, Effet »), qui ajoute des composants d'évaluation des risques à l'évaluation d'un incident. https://carnegieendowment.org/research/2020/09/the-eus-role-in-fighting-disinformation-crafting-a-disinformation-framework?lang=en


| Phase | Définition |
|--------|----------------------------------|
| Acteur | Quels sont les types d'acteurs impliqués ? Cette question peut aider à déterminer, par exemple, si l'affaire implique un acteur étatique étranger |
| Comportement | Quelles sont les activités manifestées ? Cette question peut aider à établir, par exemple, des preuves de coordination et d'inauthenticité
| Contenu | Quels types de contenu sont créés et distribués ? Cette ligne de questions peut aider à établir, par exemple, si les informations déployées sont trompeuses.|
| Degré |Quel est l'impact global de l'affaire et qui cela affecte-t-il ? Cette question peut aider à établir les préjudices réels et la gravité de l'affaire. |
| Effet | Quel est l'impact global de l'affaire et qui cela affecte-t-il ? Cette question peut aider à déterminer les préjudices réels et la gravité de l'affaire. |


## 2.4 Modèles de désinformation basés sur le comportement
Les communauté de l'infosec et de lutte contre les manipulations de l'information ont de nombreux modèles qui décrivent les comportements des créateurs d'incidents et des personnes chargées d'y répondre. Plusieurs de ces modèles, dont les Framework DISARM et MITRE & ATTACK, se concentrent sur les techniques, tactiques et procédures (TTP) utilisées par les créateurs d'incidents et les intervenants.

La plupart des efforts de NORMA ont porté sur la manière d'adapter ces modèles, et les outils qui les utilisent, aux opérations juridiques.

### 2.4.1 Modèles de réponse juridique aux manipulations de l'information

En 2021, NORMA a étudié des opérations juridiques connus pour y trouver des comportements de créateurs d'incidents, et a cherché à s'inspirer et à définir des cadres pour les modèles d'opérations juridiques en réponse à une manipulation de l'information. 

Dans le cadre de ces travaux s'attardant plus spécifiquement aux manipulations de l'information, le groupe a examiné des modèles basés sur le comportement dans les domaines de la sécurité de l'information, de l'analyse des réseaux sociaux, du marketing et de la technologie publicitaire avant d'opter pour la Cyber Killchain, le modèle ATT&CK et le modèle DISARM qui en découle, comme représentation de base pour les réponses juridiques aux manipulations de l'informations.
