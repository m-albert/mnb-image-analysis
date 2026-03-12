# Setting up a Python environment


1. [Download the repository](https://github.com/microscopy-network-basel/mnb-image-analysis/archive/refs/heads/main.zip).
2. Extract the content of the downloaded zip file.
3. Open a terminal and change to the directory.
    ```bash
    cd path/to/mnb-image-analysis-main
    ```
4. Create the Python environment.
    ```bash
    pixi install --all
    ```
    ```{admonition} What happens?
        The Python environment with all the dependencies is created in a sub-folder `.pixi`.
        You can activate the environment using:
        ```bash
        pixi shell
        ```
        And deactivate the environment with:
        ```bash
        exit
        ````
    ````

## Start the notebook

1. In a terminal within the repository folder, i.e.:
    ```bash
    cd path/to/mnb-image-analysis-main
    ```
2. Run following command to start Jupyter Lab:
    ```bash
    pixi run jupyter lab
    ```
    
This will open a browser for interactive coding in noteoboks.
