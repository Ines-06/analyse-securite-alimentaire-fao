🌍 Analyse de la sous-nutrition dans le monde

📌 Contexte

Ce projet a pour objectif d'étudier la sécurité alimentaire mondiale à partir des données de la FAO (Food and Agriculture Organization).

L'analyse cherche notamment à mieux comprendre les déséquilibres entre la production alimentaire, la disponibilité des ressources et leur accès par les populations.

Plusieurs dimensions ont été étudiées :

la population mondiale ;

la sous-nutrition ;

la disponibilité alimentaire ;

les différents usages des ressources alimentaires ;

l'aide alimentaire internationale.

🎯 Objectifs de l'analyse

L'étude permet notamment de répondre aux questions suivantes :

Quelle part de la population mondiale est en situation de sous-nutrition ?

Combien de personnes pourraient théoriquement être nourries grâce aux ressources alimentaires disponibles ?

Quelle part de la disponibilité intérieure est destinée à l'alimentation humaine, animale ou à d'autres usages ?

Comment les principales céréales sont-elles réparties entre alimentation humaine et animale ?

Quels pays présentent les taux de sous-nutrition les plus importants ?

Quels pays ont le plus bénéficié de l'aide alimentaire ?

Quels pays disposent de la plus forte ou de la plus faible disponibilité alimentaire par habitant ?

Quelle est la situation particulière de la Thaïlande concernant la production et l'exportation du manioc ?

Une analyse complémentaire de la Syrie a également été réalisée afin d'observer le lien entre conflits armés et évolution de l'aide alimentaire.

📊 Données utilisées

L'analyse repose sur quatre jeux de données issus de la FAO :

Population

Population par pays et par année.

Sous-nutrition

Nombre estimé de personnes en situation de sous-nutrition par pays.

Disponibilité alimentaire

Informations concernant notamment :

la disponibilité en kcal/personne/jour ;

la production ;

les importations et exportations ;

l'alimentation humaine ;

l'alimentation animale ;

les pertes ;

les semences ;

le traitement ;

les autres utilisations.

Aide alimentaire

Quantités d'aide alimentaire reçues par pays sur plusieurs années.

Les données sont publiques et agrégées à l'échelle des pays. Elles ne contiennent pas de données personnelles ou nominatives.

🛠️ Outils et technologies

Python

Pandas : manipulation, nettoyage et analyse des données

NumPy : calcul numérique

Matplotlib : visualisation des résultats

Jupyter Notebook : environnement d'analyse

Excel : première visualisation et compréhension des fichiers CSV

🔎 Méthodologie

L'analyse a été réalisée progressivement, en partant d'une vision globale avant d'approfondir certains sujets.

1. Exploration des données

Les différents datasets ont d'abord été étudiés afin de vérifier :

leurs dimensions ;

les types de variables ;

les valeurs manquantes ;

la structure des colonnes ;

les unités utilisées.

Des fonctions comme head(), info(), shape, count() et isna() ont notamment été utilisées.

2. Nettoyage et préparation

Plusieurs opérations ont ensuite permis d'harmoniser les données :

conversion des types avec astype() et pd.to_numeric() ;

traitement des valeurs manquantes avec fillna() ;

conversion des unités ;

renommage de certaines colonnes ;

création de nouvelles variables nécessaires aux calculs.

3. Croisement des données

Les différents datasets ont été croisés grâce à des jointures Pandas (merge), notamment entre les données de population, de sous-nutrition et de disponibilité alimentaire.

Les jointures ont principalement été réalisées sur la variable Zone, correspondant au pays.

4. Agrégation et calcul des indicateurs

Des fonctions telles que :

groupby()

agg()

sum()

sort_values()

loc

isin()

ont été utilisées pour agréger les données par pays ou par année et construire les différents indicateurs.

5. Visualisation

Plusieurs graphiques ont été réalisés avec Matplotlib afin de faciliter la comparaison et l'interprétation des résultats.

📈 Principaux résultats

🌍 Sous-nutrition mondiale

En 2017 :

environ 535,7 millions de personnes étaient en situation de sous-nutrition ;

soit environ 7,10 % de la population mondiale.

🍽️ Capacité alimentaire mondiale

En utilisant une hypothèse de consommation moyenne de 2 500 kcal par personne et par jour, les disponibilités alimentaires mondiales permettraient théoriquement de nourrir environ :

8,37 milliards de personnes.

Ce résultat reste théorique puisqu'il ne prend pas en compte les inégalités de distribution et d'accès à l'alimentation.

📦 Répartition de la disponibilité intérieure

La disponibilité intérieure mondiale se répartit notamment de la manière suivante :

Nourriture : 49,46 %

Traitement : 22,36 %

Alimentation animale : 13,23 %

Autres utilisations : 8,77 %

Pertes : 4,60 %

Semences : 1,57 %

Cette analyse montre qu'une partie importante des ressources alimentaires disponibles n'est pas directement destinée à l'alimentation humaine.

🌾 Utilisation des principales céréales

En considérant uniquement leur utilisation pour l'alimentation humaine et animale :

54,09 % sont destinées à l'alimentation humaine ;

45,91 % sont destinées à l'alimentation animale.

La répartition est donc relativement équilibrée entre ces deux usages.

🇹🇭 Étude du cas de la Thaïlande

L'analyse de la Thaïlande a permis d'obtenir les résultats suivants :

6,2 millions de personnes sous-alimentées ;

soit environ 8,96 % de la population ;

disponibilité alimentaire moyenne d'environ 2 785 kcal/personne/jour.

L'analyse du manioc montre également qu'environ 83,41 % de la production étudiée est exportée.

Ce cas permet d'illustrer qu'une disponibilité alimentaire nationale relativement élevée ne signifie pas nécessairement que toute la population bénéficie du même accès à l'alimentation.

🇸🇾 Analyse complémentaire : Syrie

Une analyse complémentaire a été menée sur l'évolution de l'aide alimentaire en Syrie.

Les données mettent en évidence l'importance de l'aide alimentaire pendant la période étudiée.

Cette analyse permet d'élargir l'étude en montrant que la sécurité alimentaire ne dépend pas uniquement de la quantité de nourriture produite : les conflits, les déplacements de population, l'accès aux ressources et la désorganisation des infrastructures peuvent également jouer un rôle majeur.

💡 Conclusion

La production alimentaire mondiale est aujourd'hui suffisante pour répondre aux besoins de la population.

Pourtant, la sous-nutrition persiste, principalement à cause d'inégalités d'accès à la nourriture, de la pauvreté et de certains contextes politiques ou de conflits.

On observe ainsi une double réalité dans le monde : certains pays manquent encore de ressources alimentaires, tandis que d'autres disposent d'une alimentation largement suffisante.

Cette analyse montre donc que l'amélioration de la sécurité alimentaire mondiale ne dépend pas uniquement de la production agricole, mais également de facteurs économiques, sociaux et politiques.

🧠 Compétences développées

Ce projet m'a permis de développer et consolider plusieurs compétences en analyse de données :

préparation et nettoyage de données ;

exploration de datasets ;

manipulation de DataFrames avec Pandas ;

traitement des valeurs manquantes ;

sélection et restriction de données ;

jointures entre plusieurs tables ;

agrégation avec groupby() et agg() ;

création d'indicateurs ;

calcul de proportions ;

classement et comparaison de données ;

visualisation avec Matplotlib ;

interprétation de résultats dans un contexte métier ;

communication des résultats à travers un support de présentation.

📁 Livrables

Le projet comprend :

un Jupyter Notebook contenant le nettoyage, les calculs, les analyses et les visualisations ;

un support de présentation synthétisant la méthodologie, les principaux résultats et les conclusions de l'étude.

Projet réalisé dans le cadre de ma formation Data Analyst.
