
---

## 2) README.md complet pour GitHub (prêt à déposer)

```markdown
# Oryntra — FiveM Utility System

**Oryntra** est un utilitaire desktop (terminal UI) conçu pour faciliter l'organisation et la gestion des ressources **FiveM**.  
Il automatise le classement des fichiers de projet (véhicules, tenues, mappings, armes) pour améliorer le workflow des développeurs.

---

## 🔹 Caractéristiques principales

- **Vehicle Organizer** — trie les `.yft`, `.ytd`, `.ydd`, `.ydr` par dossier `[vehiclename]`.  
- **Outfit Classer** — détecte `mp_m_` / `mp_f_` et range en `[male]` / `[female]` + catégories.  
- **Mapping Manager** — structure `.ymap`, `.ytyp`, `.xml`, `.meta`, `.dat`, etc.  
- **Weapons Organizer** — renomme dossiers, déplace `component*`, range par `[ydr]`, `[ytd]`, `[meta]`…  
- **Interface** — menu terminal centré, couleurs, barre de progression, logs, et support Windows native folder picker.

---

## 📦 Distribution

Les releases officielles sont fournies en `.exe` (PyInstaller, `--onefile`) dans le dossier `dist/`.  
Chaque release inclut également :
- `Oryntra_vX.Y.Z_SHA256.txt` — SHA256 checksum du binaire.
- `Oryntra_vX.Y.Z_SHA256.txt.sig` — (optionnel) signature GPG du fichier de checksum.
- Lien vers **VirusTotal** report public.

---

## 🔒 Ce n’est pas un hack — comment vérifier l’intégrité

**Pourquoi distribuer un EXE ?**  
L'exécutable permet de protéger le code source (copyright/licence) et d'assurer une installation simple pour les utilisateurs non techniques. Oryntra **n’exécute pas d’opérations réseau malveillantes** — il opère uniquement sur des fichiers locaux choisis par l'utilisateur.

**Méthodes de vérification fournies :**
1. **SHA256 checksum** — garantit que le binaire reçu est exactement celui publié.
2. **Signature GPG** (optionnelle) — prouve que la checksum vient bien de l'auteur.
3. **Authenticode / Code signing** (optionnel) — signature Microsoft pour exécutable Windows.
4. **VirusTotal public scan** — rapport antivirus du binaire.

### Vérifier le SHA256 (Windows PowerShell)
```powershell
# Calcule le SHA256 local
Get-FileHash .\Oryntra.exe -Algorithm SHA256

# Affiche le SHA256 publié
Get-Content .\Oryntra_v1.0.0_SHA256.txt
