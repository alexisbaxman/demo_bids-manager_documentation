# Installation Guide
You can install BIDS-Manager in two different ways:

````{tab-set}
```{tab-item} One-click installers (recommended)

**1. Download the ZIP package:**  
* **[📦 One-click Installers](https://github.com/ANCPLabOldenburg/BIDS-Manager/raw/main/Installers/Installers.zip
)**


**2. **Extract** the ZIP file and run the script for your operating system:**

| OS               | Script                        | How to Run                         | Duration |
|------------------|-------------------------------|------------------------------------|---------|
| **Windows 10/11**| `install_bids_manager.bat`     | Double-click                        | ≈ 5 min |
| **Linux**        | `install_bids_manager.sh`      | `./install_bids_manager.sh`         | ≈ 5 min |


```

```{tab-item} Manual Installation (advanced)

**1. Create a virtual environment**

We strongly recommend using BIDS-Manager within a **virtual environment** to avoid conflicts with system dependencies.
The One-click installer automatically creates and manages a virtual environment, meanwhile the Manual Installation requires you to create one manually. If you want to learn more about virtual environments, [click here](../extra/environment.md)

```bash
# Navigate to your target directory and create a virtual environment
python3 -m venv <env_name>

# Activate the virtual environment
source <env_name>/bin/activate
# On Windows: <env_name>\Scripts\activate

```

**2. Install BIDS Manager from GitHub**

```bash
pip install bids-manager
```


```
````

Both installation methods include all the depencies required to run the GUI and helper scripts. All core requirements are version pinned in [`pyproject.toml`](https://github.com/ANCPLabOldenburg/BIDS-Manager/blob/main/pyproject.toml) to ensure consistent installations. 

## After the installation finishes, you will find two **shortcuts** on your desktop:

| OS          | Launch                    | Uninstall                      |
|-------------|---------------------------|--------------------------------|
| **Windows** | `run_bidsmanager.bat`      | `uninstall_bidsmanager.bat`    |
| **Linux**   | **BIDS Manager** (launcher)| `uninstall_bidsmanager.sh`     |


