# YOLOv3 Object Detection

Une implémentation modulaire de YOLOv3 (You Only Look Once v3) pour la détection d'objets sur le dataset PASCAL VOC, construite avec PyTorch.

## Fonctionnalités

- Architecture complète YOLOv3 avec Darknet-53 comme backbone
- Détection multi-échelle pour identifier des objets de différentes tailles
- Support pour le dataset PASCAL VOC avec 20 classes
- Outils de visualisation pour comparer annotations et prédictions
- Pipeline d'entraînement et de validation complet
- Implémentation du mécanisme d'anchors et de la fonction de perte YOLO
- Post-traitement avec suppression non-maximale (NMS)

## Structure du projet

```
├── config.py       # Configuration et constantes
├── model.py        # Architecture YOLOv3
├── dataset.py      # Chargement des données PASCAL VOC
├── utils.py        # Fonctions utilitaires et post-traitement
├── loss.py         # Fonction de perte YOLOLoss
├── train.py        # Fonctions d'entraînement
├── visualize.py    # Outils de visualisation
└── main.py         # Script principal avec interface interactive
```

## Technologies utilisées

- Python 3.10+
- PyTorch 2.0+
- PASCAL VOC 2012 dataset
- Matplotlib pour la visualisation
- NumPy pour le traitement numérique

## Installation et utilisation

```bash
# Cloner le dépôt
git clone https://github.com/votre-username/yolov3-object-detection.git
cd yolov3-object-detection

# Installer les dépendances
pip install torch torchvision matplotlib numpy tqdm

# Exécuter le programme principal
python main.py
```

Le script proposera différentes options:
1. Visualiser des exemples du dataset
2. Entraîner un nouveau modèle
3. Charger un modèle pré-entraîné
4. Visualiser les prédictions du modèle

## Perspectives d'amélioration

- Ajout de l'augmentation de données
- Support pour des datasets personnalisés
- Implémentation de métriques d'évaluation (mAP)
- Export vers des formats de déploiement (ONNX, TorchScript)
