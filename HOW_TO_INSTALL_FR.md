
Instructions d'installation et de configuration
===============================================

Suivez les instructions pour votre système d'exploitation ci-dessous.

- [Windows 10+](#Windows)
- [Mac OS X](#GNU-Linux-ou-Mac-OS-X)
- [GNU Linux](#GNU-Linux-ou-Mac-OS-X)


Windows
-------------------

**Tout d'abord, assurez-vous de connaître votre nom d'utilisateur Windows.**

- *Si vous ne connaissez pas votre nom d'utilisateur Windows, tapez plutôt ce qui suit et appuyez sur ENTRÉE :*
```
whoami
```

Le résultat de cette commande pourrait être quelque chose comme `organization
nom_utilisateur`; votre nom d'utilisateur Windows, dans cet exemple, serait `nom_utilisateur`.

**Ensuite, nous devons installer Python.**

- [Téléchargez la dernière version stable pour Windows.](https://www.python.org/downloads/windows/)

**Ensuite, vous devez installer les bibliothèques Python que nous allons utiliser.**

- Ouvrez Windows PowerShell ; à partir du menu **"Démarrer"**, commencez à taper "PowerShell" et cliquez sur l'icône de l'application lorsqu'elle apparaît.
- Une interface en ligne de commande devrait apparaître. Elle devrait ressembler *à peu près* à la capture d'écran ci-dessous, bien que le texte dans votre fenêtre puisse être légèrement différent.

![](./images/capture_OSGeo4W.png)

- Tapez ce qui suit et appuyez sur ENTRÉE pour installer les bibliothèques Python nécessaires :
```
pip install numpy scipy notebook xarray earthaccess h5py h5netcdf cartopy dask
```


### Démarrage de Jupyter Notebook

**Pour lancer Jupyter Notebook,** changez d'abord votre répertoire de travail en votre dossier personnel en tapant ce qui suit, en veillant à remplacer `nom_utilisateur` par votre nom d'utilisateur Windows réel :
```
cd C:/Users/nom_utilisateur
```

Vous pouvez démarrer Jupyter Notebook en tapant ce qui suit, puis appuyez sur ENTRÉE :
```
python -m notebook
```


### Alternatives à `pip` sous Windows

Nous ne recommandons pas d'utiliser `conda` ou `miniconda`. Si vous souhaitez utiliser un autre gestionnaire de paquets Python, nous recommandons `mamba`, installé via `mambaforge`.

- Téléchargez et exécutez l'installateur `mambaforge`, [ici.](https://github.com/conda-forge/miniforge#mambaforge)
- Lancez le **Miniforge Prompt** en tapant "miniforge" à partir du menu Démarrer ou du menu de recherche.
- À l'invite de commande de Miniforge, tapez ce qui suit, en appuyant sur ENTRÉE après chaque ligne.

```
mamba install numpy scipy notebook xarray earthaccess h5py h5netcdf cartopy pyproj dask
pip install --force pillow
```


GNU Linux ou Mac OS X
---------------------

Python et `pip` devraient déjà être installés. Depuis le **Terminal** de Mac OS X ou Linux, vous pouvez installer les dépendances Python en exécutant la commande suivante :

```sh
pip install numpy scipy notebook xarray earthaccess h5py h5netcdf cartopy dask
```


### Démarrage de Jupyter Notebook

**Pour lancer Jupyter Notebook,** tapez ce qui suit dans la ligne de commande, en vous assurant que votre répertoire de travail actuel est celui où vous souhaitez que l'arborescence des fichiers Jupyter commence :

```sh
jupyter notebook
```


### Alternatives à `pip` sous Mac OS X

**Sous Mac OS X :**

- Ouvrez une nouvelle fenêtre de **Terminal**.
- Installez `mamba` ("miniforge") en [suivant les instructions ici.](https://github.com/conda-forge/miniforge?tab=readme-ov-file#unix-like-platforms-mac-os--linux)
- Si `mamba` ("miniforge") a été installé dans votre répertoire personnel, par exemple `/Users/nom_utilisateur/miniforge3`, où `nom_utilisateur` est votre nom d'utilisateur, vous pouvez *initialiser* `mamba` avec :
```
/Users/nom_utilisateur/miniforge3/bin/mamba init
```
- Ensuite, chaque fois que vous souhaitez utiliser ou installer des modules Python, ouvrez une fenêtre de **Terminal** et tapez :
```
mamba activate
```
- Si vous préférez que l'environnement `(base)` ne soit pas initialisé par défaut à chaque fois que vous ouvrez un shell, modifiez cette configuration (il s'agit en fait d'une commande pour `miniforge`, même si elle commence par `conda`) :
```sh
conda config --set auto_activate_base false
```
