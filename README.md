<img width="1870" height="797" alt="image" src="https://github.com/user-attachments/assets/508cfdc9-5e89-4368-8140-2f66bfdac2d4" /># 🛡️ Safe Asset Cleaner

**Safe Asset Cleaner** is a comprehensive and safe tool designed to optimize your Unity project by removing unused assets, duplicates, and empty folders. It features a robust **Auto-Backup & Undo system**, allowing you to clean your project without the fear of breaking it.

<img width="1870" height="797" alt="image" src="https://github.com/user-attachments/assets/3a051fff-0423-406d-b996-54c42ed00902" />


* **🛡️ Safety First:** Automatic `.unitypackage` backups before deletion and a **One-Click Undo** button.
* **🔍 Unused Asset Finder:** Deep scans scenes, prefabs, and build settings to find truly unused files.
* **👯 Duplicate Finder:** Uses **MD5 hashing** to detect identical files even if they have different names.
* **📂 Empty Folder Remover:** cleans up your project hierarchy instantly.
* **🔗 Advanced Reference Finder:** Finds exactly **which GameObject** and **Component** is referencing a specific asset.
* **🚀 Smart UX:** Double-click any item in the list to ping it in the Project View.

---

## 📦 Installation

1.  Purchase and download the asset from the [Unity Asset Store](https://assetstore.unity.com/packages/slug/351938).
2.  Import the package into your Unity project via Package Manager.
3.  Go to **Tools > asdlk50 > Project Cleaner** to open the window.

---

## 📖 How to Use

### 1. Finding & Removing Unused Assets
Clean up assets that are not referenced by any Scene, Prefab, or Script.

1.  Open the **Unused Assets** tab.
2.  Click **"Scan Unused Assets"**.
3.  Review the list. (Double-click an item to locate it).
4.  Click **"Delete Selected Assets"**.
    * *A backup is automatically created before deletion.*

> **⚠️ Note:** Assets loaded dynamically via code (e.g., `Resources.Load`, `Addressables`) might be detected as unused. Please add their folders to the **Ignore List** in the Settings.

### 2. Removing Empty Folders
Keep your project structure clean.

1.  Open the **Empty Folders** tab.
2.  Click **"Scan Empty Folders"**.
3.  Click **"Delete Selected Folders"**.

> **Note:** Deletion of empty folders **cannot be undone** and does not create a backup, as they contain no data.

### 3. Finding Duplicates
Find assets that are identical in content but have different names or paths.

1.  Open the **Duplicate Assets** tab.
2.  Click **"Scan Duplicate Assets"**.
3.  The tool groups duplicates by hash.
4.  Click **"Auto Select (Keep One)"** to automatically mark copies for deletion while keeping the original.
5.  Click **"Delete Selected Duplicates"**.

### 4. Reference Finder (Deep Scan)
Find where a specific asset is being used in your project.

1.  Open the **Ref Finder** tab.
2.  Drag and drop an asset into the **Target Asset** field.
3.  Click **"Find References (Deep Scan)"**.
4.  The result list shows:
    * **Scenes:** Shows the specific **GameObject name** and **Component**.
    * **Prefabs:** Shows the prefab path.
5.  **Double-click** any result to highlight the object in the Hierarchy or Project view.

---

## ⚙️ Settings & Safety

Click the **"Settings & Safety"** foldout at the top of the window.

* **Scan All Scenes:** Check this to include scenes not in the Build Settings (Recommended).
* **Safe Filters:** Ignore Materials or ScriptableObjects automatically.
* **Ignore List (Whitelist):** Add specific folders or files to exclude them from scanning.
    * *System folders like `ProjectSettings`, `Packages`, and `Backups` are ignored by default.*

---

## ↩️ Backup & Undo System

Your safety is our priority.

1.  **Auto-Backup:** Every time you delete assets (Unused or Duplicates), a backup file is created at:
    `Assets/asdlk50/ProjectCleaner/Backups/LastAutoBackup.unitypackage`
2.  **Undo:** A green **"Undo Last Delete"** button appears at the bottom of the window after deletion. Clicking it will immediately restore the deleted files.

---

## 🛠️ Technical Details

* **Unity Version:** 2021.3 LTS or newer.
* **Compatibility:** Works with Built-in, URP, and HDRP.
* **No DLLs:** Full C# source code included.

## 📄 License & Terms

This asset is a **paid package** available exclusively on the **Unity Asset Store**.
The source code and assets are protected by the **Unity Asset Store End User License Agreement (EULA)**.

### 🚫 Restrictions
* **No Redistribution:** You may **NOT** share, redistribute, or resell this package (or its source code) in any form.
* **Public Repository:** Do not upload the full source code of this asset to a public repository (GitHub, GitLab, etc.) where it can be downloaded for free.

### ✅ Usage
* You are free to modify the source code for use in your own commercial or non-commercial projects **after purchasing a license** from the Unity Asset Store.

---
**Copyright © 2026 asdlk50. All rights reserved.**

## 📧 Support
If you have any questions or find a bug, please contact us:
* **Email:** asdlk50@gmail.com
