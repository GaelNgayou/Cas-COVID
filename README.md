L'analyse portait sur le rapport des cas Covid dans 230 pays et sur les décès. Tout d'abord j'ai importé le fichier (téléchargé sur Kaggle) dans Colab pour y faire du nettoyage et la transformation des données avec Python.
J'ai évalué le nombre de valeurs aberrantes (Nan) pour orienter mes actions. J'ai procédé par interpolation pour remplacer les valeurs avec les chiffres qui se rapprocheraient le mieux de la réalité. Après avoir essayé plusieurs méthodes d'interpolation, il restait encore des Nan représentant 7.26% des données. J'ai jugé utile de les remplacer par des 0 et de les isoler lors de l'analyse, vu qu'elles portaient sur des pays qui avaient initialement peu de cas et dont les autres informations n'étaient pas renseignées.
J'ai converti les colonnes en entiers pour avoir des informations harmonieuses et plus digestes lors de l'analyse. J'ai concatené les colonnes, vu qu'au départ il a fallu extraire celles sur lesquelles il fallait faire des conversion (en int64) et interpolation.
Et enfin j'ai exporté le nouveau fichier .csv pour en faire l'analyse sur PowerBI
