# Projet finale algo


**chemin efficace**

Il s'agit d'un programe, un petit jeu, qui implémente un algorithme de recherche de chemin le plus rapid,  
en utilisant l'algorithme A* (A-Star), priorityQueue  dans un tableau d'Array. J'ai utilisé une liste liée.
Le patron de conception utilisé , le Singleton.  il y a aussi la possibilite de change la  langue en francais, et 
Anglais par defaut .
Donc, le but est de trouver le chemin le plus court entre deux points dans une grille de 19x19. Les nœuds de la grille sont 
reliés entre eux pour former un graphe non-orienté.

L'interface graphique permet à l'utilisateur de sélectionner les points de départ et d'arrivée, ainsi que
d'ajouter des obstacles en cliquant et en faisant glisser la souris sur la grille.

**Complexité**
pour ce qui attrait à A* : 

tout d'abord une classe qui definit , les arretes du graphe, Cette classe contient des attributs qui représentent 
la distance entre les nœuds connectés par l'arête (g), les deux nœuds eux-mêmes (a et b) et des méthodes 
pour récupérer ou définir ces attributs. De plus, la méthode "getOppositeNode" permet de récupérer le nœud opposé 
à celui fourni en argument. La méthode "toString" est utilisée pour renvoyer une chaîne de caractères 
qui décrit l'objet Edge.
Étant donnée que je les arretes du graphe ne change pas vraiment.. il n a pas de calcul a ce niveau
cependant un graphe  si on ajoute les methode comme AddEDGE, RemoveEDDGE, Remove ..la complicité va être de :

AddEdge: O(1)
Remove: O(|V| + |E|)
Remove edge: O(|V| + |E|)
Len: O(1)

une classe , graphe qui est utilisée pour stocker et gérer les nœuds et les arêtes d'un graphe. 
Il utilise l'algorithme A* pour trouver le chemin le plus court entre deux nœuds du graphe.

addNode : O(1) vu qu'elle ajoute juste un noeud.
link() : O(1)
findPath() O(|E| log |V|) 

une classe, Heuristic , pour définir une méthode de calcul de la distance heuristique entre deux nœuds d'un graphe

O(1), vu qu elle contient qu'une methode abstraite

une classe node, contient pas mal de methode . dont l'en premiere qui gerer son  états du node/noued.( ouvert, 
pas visité ou bloqué)

setState(State state) : O(1)
setIcon(Image icon) : O(1)
setBlocked(boolean blocked) : O(1)
setG(double g) : O(1)
setH(double h) : O(1)
setBackPathNode(Node backPathNode) : O(1)
addEdge(Edge edge) : O(1)
getF() : O(1)
retrievePath(List<Node<T>> path) : O(n) où n est le nombre de noeuds dans le chemin
compareTo(Node o) : O(1)
toString() : O(1)



**Utilisation**

**Comment exécuter le programme**
 
Ouvrir une invite de commande ou un terminal dans le dossier racine du projet : javac *.java

Compiler les fichiers source et le lancer a partir du fichier View.. 

Pour exécuter les exemples de code,  nous avons utulisé intellij.
  En Java.

resulat: 

![image](https://user-images.githubusercontent.com/111302767/226074293-55f7d932-4972-4bb1-b804-1a5ed6db02a0.png)







**État du projet :**

completé 
