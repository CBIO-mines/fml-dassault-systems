# Fondamentaux du Machine Learning 

Ce répertoire contient les notebooks qui accompagnent la formation « Fondamentaux du Machine Learning ».

## Librairies
Ces notebooks ont été créés avec Python 3.13.2 et les librairies suivantes :
* matplotlib 3.10.1
* numpy 2.2.4
* pandas 2.2.3
* scikit-learn 1.6.1

Pour utiliser les même librairies, utilisez le fichier `package_list.yml` :
* Avec Anaconda, suivez la section "Importing an environment" [du tutoriel](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/). 
* En ligne de commande, utilisez
```bash
   conda env create -f package_list.yml -n introml
   conda activate introml
   pip install torch --index-url https://download.pytorch.org/whl/cpu
```

## Contenus
* Cours 1 : prise en main de `scikit-learn`
* Cours 2 : sélection de modèle, régularisation
* Cours 3 : réduction de dimension et clustering
* Cours 4 : arbres et modèles ensemblistes
* Cours 5 : entrainement de réseaux de neurones


## Utilisation avancée (git et nbstripout)
Pour faciliter le contrôle de version avec de notebooks jupyter, vous pouvez utiliser [`nbstripout`](https://pypi.org/project/nbstripout/), qui nettoie votre notebook (en particulier en enlevant les cellules de sortie) : 
avant de faire un commit,
```bash
nbstripout <nom_du_notebook>.ipynb
```
vous pouvez utiliser `git diff <nom_du_notebook>.ipynb` avant votre comit pour vérifier les modifications.
