# Unreal Engine Git Templates

Recommended `.gitignore` and `.gitattributes` templates for Unreal Engine projects.  
These templates are tailored for projects using **Git LFS** to efficiently manage large binary assets.

📦 Repository: [sungkukpark/unrealengine-git-templates](https://github.com/sungkukpark/unrealengine-git-templates.git)

---

## ✨ Features

### .gitignore Highlights

- Excludes common Unreal build artifacts and caches:
  - `Binaries/`, `Intermediate/`, `DerivedDataCache/`, `Saved/`
- Prevents accidental commits of platform-specific or temporary files
- Keeps the repository clean and focused on reproducible sources

### .gitattributes Highlights

- Enforces proper line endings:
  - `*.bat` → CRLF
  - `*.sh` → LF
- Configures **Git LFS** for Unreal Engine assets and other large/binary files:
  - `.uasset`, `.umap`, `.fbx`, `.wav`, `.png`, `.dll`, `.exe`, `.zip`, etc.
- Ensures consistent handling of binaries and media across platforms

---

## 🚀 Usage

1. Copy the template files into the root of your Unreal Engine project:

   ```bash
   curl -O https://raw.githubusercontent.com/sungkukpark/unrealengine-git-templates/main/.gitignore
   curl -O https://raw.githubusercontent.com/sungkukpark/unrealengine-git-templates/main/.gitattributes
   ```

2. Install Git LFS (if not already installed):

   ```bash
   git lfs install
   ```

3. Stage and commit the templates first to ensure LFS tracking is applied correctly:

   ```bash
   git add .gitignore .gitattributes
   git commit -m "Add Unreal Engine Git templates (.gitignore, .gitattributes)"
   ```

---

## 🛠️ Why these templates?

Unreal Engine projects generate many intermediate files and large binary assets that should not be stored directly in Git.  
These templates provide:

- A clean Git history by ignoring unnecessary files
- Git LFS tracking for large assets to keep the repo lean
- Cross-platform consistency for scripts and binaries
- A reliable starting point for both solo developers and teams

---

## 📖 References

- [Unreal Engine Documentation: Using Git as Source Control](https://docs.unrealengine.com/5.0/en-US/using-git-as-source-control-in-unreal-engine/)
- [Git LFS Documentation](https://git-lfs.github.com/)
- [Git Attributes Documentation](https://git-scm.com/docs/gitattributes)
- [Git Ignore Documentation](https://git-scm.com/docs/gitignore)

---

## 📌 License

This repository is distributed under the MIT License.  
Feel free to use, modify, and share.

---

## 📂 Included Template

- `.gitignore`
- `.gitattributes`
