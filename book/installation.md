# Installation Guide
You can install BIDS-Manager in two ways:

## 1. One-click installers (recommended)

### 1. **Download** the ZIP package:  
   **[📦 One-click Installers](https://github.com/ANCPLabOldenburg/BIDS-Manager/raw/main/Installers/Installers.zip
)**
<br>

### 2. **Extract** the ZIP file and run the script for your operating system:

| OS               | Script                        | How to Run                         | Duration |
|------------------|-------------------------------|------------------------------------|---------|
| **Windows 10/11**| `install_bids_manager.bat`     | Double-click                        | ≈ 5 min |
| **Linux**        | `install_bids_manager.sh`      | `./install_bids_manager.sh`         | ≈ 5 min |

<br>

### 3. After the installation finishes, you will find two **shortcuts** on your desktop:

| OS          | Launch                    | Uninstall                      |
|-------------|---------------------------|--------------------------------|
| **Windows** | `run_bidsmanager.bat`      | `uninstall_bidsmanager.bat`    |
| **Linux**   | **BIDS Manager** (launcher)| `uninstall_bidsmanager.sh`     |

---


## 2. Manual Installation (advanced)

### 1. **Create a virtual environment**

We strongly recommend using BIDS-Manager within a **virtual environment** to avoid conflicts with system dependencies.
The One-click installer automatically creates and manages a virtual environment, meanwhile the Manual Installation requires you to create one manually. If you want to learn more about virtual environments, [click here](../extra/environment.md)

```bash
# Navigate to your target directory and create a virtual environment
python3 -m venv <env_name>

# Activate the virtual environment
source <env_name>/bin/activate
# On Windows: <env_name>\Scripts\activate

```

### 2. **Install BIDS Manager from GitHub**

```bash
pip install bids-manager
```

The pip installation includes all the depencies required to run the GUI and helper scripts. All core requirements are version pinned in [`pyproject.toml`](https://github.com/ANCPLabOldenburg/BIDS-Manager/blob/main/pyproject.toml) to ensure consistent installations. 

```{admonition} List of dependencies
:class: dropdown
* pydicom==3.0.1
* pandas==2.3.1
* PyQt5==5.15.11
* PyQtWebEngine==5.15.7
* heudiconv-ancp
* dcm2niix==1.0.20250506
* nibabel==5.3.2
* numpy==2.2.6
* psutil==7.0.0
* matplotlib==3.10.3
* joblib==1.4.2

``` 



