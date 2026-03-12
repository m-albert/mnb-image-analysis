# Installing Python

To run the Python Jupyter notebooks used in this course, you need to install Python locally on your computer.

We recommend using `Pixi` to manage your Python environment.

```{tip}
You will be using a terminal for the setup: 
- **Windows**: Open the "Command Prompt" from your start menu
- **Mac OS**: Open Terminal (you can search for it in spotlight - cmd + space)
- **Linux**: Open your terminal application
```

## Pixi installation

The official installation instructions can be found [here](https://pixi.prefix.dev/latest/installation/).

`````{tab-set}
```{tab-item} Linux & macOS
1. Run the following command in your terminal:

    ```bash
    curl -fsSL https://pixi.sh/install.sh | sh
    ```

    If your system doesn't have `curl`, you can use `wget`:

    ```bash
    wget -qO- https://pixi.sh/install.sh | sh
    ```

    ```{admonition} What does this do?
        The above invocation will automatically download the latest version of `pixi`, extract it, and move the `pixi` binary to `~/.pixi/bin`.
        The script will also extend the `PATH` environment variable in the startup script of your shell to include `~/.pixi/bin`.
        This allows you to invoke `pixi` from anywhere.
    ```

```

```{tab-item} Windows
1. [Download installer](https://github.com/prefix-dev/pixi/releases/latest/download/pixi-x86_64-pc-windows-msvc.msi).

    Or run:

    ```powershell
    powershell -ExecutionPolicy Bypass -c "irm -useb https://pixi.sh/install.ps1 | iex"
    ```

    ```{admonition} What does this do?
        The above invocation will automatically download the latest version of `pixi`, extract it, and move the `pixi` binary to `%UserProfile%\.pixi\bin`.
        The command will also add `%UserProfile%\.pixi\bin` to your `PATH` environment variable, allowing you to invoke `pixi` from anywhere.
    ```
`````

Now restart your terminal or shell to make the installation take effect.
