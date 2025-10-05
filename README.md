# 🛣️ SafeWay – Hackathon Sopra Steria In’Auvergne 2024  
###  Prix du Jury Fonctionnel  

**SafeWay** est une application web développée en 24 heures lors du **Hackathon Sopra Steria In’Auvergne 2024**.  
Elle vise à **sécuriser les trajets urbains** des piétons et cyclistes en proposant des **itinéraires optimisés selon le niveau de sécurité**, basé sur les **avis des utilisateurs** et des **données locales de dangerosité**.

---

## Objectif du projet  
L’objectif principal de **SafeWay** est d’améliorer la sécurité des déplacements en milieu urbain, en permettant à chacun de choisir un chemin non seulement rapide, mais aussi **plus sûr**.  
L’application combine **cartographie interactive**, **analyse de graphes** et **avis communautaires** pour recommander le trajet le plus sécurisé entre deux points.

---

##  Fonctionnalités principales  
- **Affichage interactif de la carte** (via Folium / OpenStreetMap)  
- **Recherche d’itinéraires** entre deux adresses  
- **Algorithme de Dijkstra** adapté avec un **coût de sécurité personnalisé**  
- **Système d’avis des utilisateurs** sur la sécurité de certaines zones  
- **Visualisation des zones à risque** (couleur et intensité selon les signalements)  
- **Mise à jour dynamique du graphe** selon les retours de la communauté  

---

##  Architecture technique  
- **Frontend** : Streamlit (interface utilisateur)  
- **Backend** : Python (calculs d’itinéraires et gestion des graphes)  
- **Cartographie** : Folium, OpenStreetMap  
- **Algorithme** : Dijkstra avec pondération personnalisée :  
  \[
  \text{coût} = \text{distance} \times (\alpha + 1)
  \]
  où **α** représente le niveau de danger perçu.  

---

##  Exemple d’utilisation  
1. L’utilisateur entre son point de départ et sa destination.  
2. SafeWay affiche plusieurs trajets possibles avec un **indice de sécurité**.  
3. L’utilisateur peut laisser un **avis** sur un segment de trajet (ex : “rue mal éclairée”).  
4. Le graphe s’ajuste automatiquement pour recommander des **chemins plus sûrs**.  
 



##  Perspectives d’évolution  
- Intégration de **données publiques de sécurité urbaine** (police, mairie, etc.)  
- Application mobile (Flutter / React Native)  
- Amélioration du scoring de sécurité via **Machine Learning**  
- Ajout de **trajets adaptés aux personnes à mobilité réduite**

---

## Technologies utilisées  
- **Langage** : Python  
- **Librairies** : Streamlit, Folium, NetworkX, Geopy, Pandas  
- **Données** : OpenStreetMap + entrées utilisateurs  

---
## 🎥 Démonstration

 
[demoSafeWay.mp4](demoSafeWay.mp4)

---

