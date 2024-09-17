# Devoir 2

## Installation

### Étape 0: Cloner et entrer dans le répertoire

On commence par clôner le répertoire, and on entre dans le nouveau répertoire

```
git clone https://github.com/BapRoyer/devoir2git.git
cd devoir2git
```

### Étape 1: Créer un environnement virtuel


On crée un environnement virtuel appelé `.phq598-devoir2`, en utilisant `venv` (recommandé):

```
python -m venv .phq598-devoir2
```

<!-- You might have to replace `python` by `python2` or `python3` depending on your Python installation. -->
À noter: Pulser ne fonctionne pas avec conda

### Étape 2: Activer l'environnement

Sur Windows

```
# Dans cmd.exe
.phq598-devoir2\Scripts\activate.bat
# Dans PowerShell
.phq598-devoir2\Scripts\Activate.ps1
```
Sur Linux et MacOS:

```
source .phq598-devoir2/bin/activate
```

### Étape 3: Installer les librairies avec `pip`

Installer la librairie `pulser` et les autres librairies requises

```
pip install -r requirements.txt
```

### Étape 4: Installer jupyter notebook

On aura besoin de jupyter notebook:

```
pip install notebook
```

#### Étape 4.1: Adding the new environment to Jupyter notebook

Il faut ajouter le nouvel environnement au jupyter notebook
<!-- If you created a new virtual environment, you'll need to add it as a new kernel in Jupyter notebook. To do so, we use `ipykernel`: -->

```
python -m ipykernel install --user --name=.phq598-devoir2
```
<!-- We now have a new kernel called `.phq598-devoir2` inside of our notebooks. -->


### Étape 5: Éxecuter le code

Finalement, on exécute le code

```
jupyter notebook
```

<!-- After opening a notebook, make sure the kernel is set to `.ieee-venv`. -->