# Project_NLP_MVA_23
Repository for the Project of Algorithms for Speech and Natural Language Processing 




# Liste des choses qui restent à faire : 


- Faire tourner le code sur tout ce qui reste 
   - chaque tache hongroise avec un des différents LLM 
   - Pareil pour les tâches françaises
   - Faire un tableau des résultats
- Finir de modifier le rapport pour inclure les valeurs quyantitatives de performance par exemple.
- Clean le github et y insérer tout les résultats 










lien de l’article : https://arxiv.org/pdf/2001.07676.pdf
Ok en faite l’article au dessus est juste la verion précédente de notre article.
Je ne comprends pas pourquoi c’est cet article qui est utilisé ? On fait pas justement : 
https://arxiv.org/pdf/2009.07118.pdf



Lien du Google Colab : 

https://colab.research.google.com/drive/1zd60dwooww8VV0NCRib-pO9FdeyT01Jv#scrollTo=wxfFVBPrZ5lZ




Lien de téléchargement du dataset MNLI : 
https://cims.nyu.edu/~sbowman/multinli/multinli_1.0.zip

Lien avec la liste de tous les datasets utilisés : https://paperswithcode.com/paper/it-s-not-just-size-that-matters-small

Vidéo youtube importante : 
https://www.youtube.com/watch?v=P7Rav5tK3Y0


Autre vidéo importante : 

https://youtu.be/01jRE9noSWw

# Une approche naive utilisation du PET avec BERT comme PLM (pck l'on sait que BERT marche ... XLM-roberta non).

# Très important :

On a voulu testé dans le verbalizer le mot "mauvais". Or le mot "mauvais est enfaite tokenizé en plusieurs bouts. AssertionError: Verbalization "mauvais" does not correspond to a single token, got ['ma', '##u', '##va', '##is']



Je décide dopnc d'utilise le mot 'nul'
