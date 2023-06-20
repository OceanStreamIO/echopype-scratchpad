# scratchpad
Experiments with echopype
This repository is designed to help users familiarize themselves with echopype.
"Echopype is a package built to enable interoperability and scalability in ocean sonar data processing. These data are widely used for obtaining information about the distribution and abundance of marine animals, such as fish and krill." [echopype](https://echopype.readthedocs.io/en/stable/index.html)

### Installation
1. Create a virtual environment:
    ```bash
    $ python -m venv .venv
    ```
    This command creates a venv in the .venv directory.

2. Activate the virtual environment:
* On Linux and MacOS, we activate our virtual environment with the `source` command:
    ```bash
    $ source <directory>/bin/activate
    ```
* On Windows:
    ```bash
    # In cmd.exe
    $ env\Scripts\activate.bat
    # In PowerShell
    $ venv\Scripts\Activate.ps1
    ```

3. Install the dependencies:
    ```bash
    $ pip install -r requirements.txt
    ```

4. Create a new kernel with a desired name:
    ```bash
    $ python -m ipykernel install --user --name=new_kernel_name
    ```

5. Open a jupyter notebook
    ```bash
    $ jupyter notebook
    ```

