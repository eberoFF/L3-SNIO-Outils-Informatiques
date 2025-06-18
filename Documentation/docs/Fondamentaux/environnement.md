# 🛠️ Configuration de l'environnement

!!! tip "Recommandé"
    Utilisez Linux pour une compatibilité optimale

## Dual Boot vs VM

```mermaid
pie
    title Choix d'Installation (Étudiants 2023)
    "Dual Boot" : 65
    "Machine Virtuelle" : 25
    "Cloud" : 10
```

## Commandes Essentielles

# Mettre à jour les paquets

sudo apt update && sudo apt upgrade -y

# Installer Jupyter Lab

pip install jupyterlab
julia -e 'using Pkg; Pkg.add("IJulia")'

!!! warning "Attention"
Les machines virtuelles peuvent avoir des problèmes de performance avec Julia.