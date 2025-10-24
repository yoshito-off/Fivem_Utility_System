# 💠 Oryntra — FiveM Utility System

> **Oryntra** est un utilitaire complet et professionnel destiné aux développeurs et créateurs de serveurs **FiveM**.  
> Il permet d’organiser automatiquement vos ressources *(véhicules, mappings, tenues, armes, etc.)* en un seul clic via une interface console claire et rapide.

---

## ⚙️ Fonctionnalités principales

🚗 **Vehicle Organizer** — Classe et trie les fichiers `.yft`, `.ytd`, `.ydd`, `.ydr`, etc.  
🧥 **Outfit Classer** — Organise les modèles et textures par genre et catégorie.  
🗺️ **Mapping Manager** — Structure automatiquement les fichiers `.ymap`, `.ytyp`, `.xml`, `.meta`, `.dat`…  
🔫 **Weapons Organizer** — Range les fichiers d’armes et leurs composants.  
⚡ **Interface Oryntra** — Menu terminal moderne, fluide et centré.

---

## 🌟 Points forts

🖥️ Interface console claire et lisible  
🪟 Compatible **Windows 10 / 11**  
📜 Génération automatique de logs détaillés  
📦 Fichier `.exe` unique — **aucune installation requise**  
🔒 Code local : aucune connexion réseau, pas de collecte de données  

---

## 🔐 Sécurité & Transparence

**Oryntra n’est pas un hack, un cheat ou un exécutable dangereux.**  
Il s’agit d’un outil de **gestion locale de fichiers** destiné aux créateurs FiveM.  
Le binaire `.exe` est simplement fourni pour :
- protéger le **code source et les droits d’auteur**,
- éviter la diffusion non autorisée,
- faciliter l’installation pour les utilisateurs.

Chaque version publiée comprend des **outils de vérification d’intégrité et d’authenticité**.

---

## 🛡️ Vérification de l’exécutable

### 🔸 1. Vérification de l’intégrité (SHA256)
Chaque release inclut un fichier `Oryntra_vX.Y.Z_SHA256.txt` contenant le hash du `.exe`.

**→ Pour vérifier (sous PowerShell) :**
```powershell
Get-FileHash .\Oryntra.exe -Algorithm SHA256
Get-Content .\Oryntra_v1.0.0_SHA256.txt
