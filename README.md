
# Builder Telegram Bot Tagging


## Roadmap

- About
- Tech
- Demo
- Installation
- Run locally
- Documentation

## About

"Builder Telegram Bot Tagging" is a script for building a "Telegram Bot Tagging" project for Linux or Windows.

## Tech Stack

- python(v3.11.3)(pyinstaller(v5.13.0), pywin32(v306))
- operating systems(Windows, Linux)

## Demo

### Windows:

- Default mode (for the current machine architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/edf2cc1f-28df-4439-a8b8-79db31de5524

- Custom mode (you will choose the architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/afb3a4b6-bcf3-4f73-8a0d-8d159d75d29e

- All mode (for both {X32} and {X64} on the current machine architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/390f21da-97c1-4677-897d-97ca13127293

### Linux:

- Default mode (for the current machine architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/ca72c759-4905-4f38-95fe-59a879f1bd25

- Custom mode (you will choose the architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/22b4d2b5-54cf-426e-98fe-158c3f828d6a

- All mode (for both {X32} and {X64} on the current machine architecture)

https://github.com/cppVolodya/text_editor/assets/103601559/e53ee80b-2af9-4e70-a9ce-606b4d379562

## Installation

#### Before performing the following steps, you need to install the necessary software for your operating system, so refer to the "documentation" heading at the very end. To build the project, you need to perform the following steps:

1. To get started, you need to download the Python interpreter:

```bash
  https://www.python.org/downloads/
```

2. After installing the interpreter, it is advisable to restart the computer. Then you need to run the main script through the console (Note: you need to run the python script in the "telegram_bot_tagging" project, because this script is designed to build this project, not another one):

```bash
  python telegram_bot_tagging/build_project.py
                        or
  python3 telegram_bot_tagging/build_project.py
```

3. Then you need to follow the instructions of the script.

## Run Locally

#### In order not to download the Python interpreter, you can use a ready-made binary file:

1. In the "telegram_bot_tagging" directory, in addition to the Python script, there are also ready-made binary (executable) files. Therefore, you need to run such command through the console, depending on your operating system:

```bash
  For Windows:
    telegram_bot_tagging/build_project.exe

  For Linux:
    telegram_bot_tagging/build_project
```

2. Then you need to follow the instructions of the script.

## Documentation

#### To successfully run the script and build the project, you must first download a number of packages or programs, depending on your operating system.

#### Windows:

- [WinRar](https://www.win-rar.com/download.html?&L=0) - download WinRar or 7-Zip(WinRar or 7-Zip or Git)

- [Git](https://git-scm.com/downloads) - download git(WinRar or 7-Zip or Git)

- [Сmake](https://cmake.org/download/) - download cmake, the minimum version you should download: 3.22.1

- [Microsoft Visual Studio](https://visualstudio.microsoft.com/downloads/) - download msvc then select package: c++ desktop

- [Vcpkg](https://vcpkg.io/en/getting-started) - download vcpkg (using git or go to https://github.com/Microsoft/vcpkg.git to download a rar or zip file), then you need to run the initial script to create vcpkg(.\vcpkg\bootstrap-vcpkg.bat). Next, you will need to install certain packages, namely: sqlitecpp and tgbot-cpp, as well as choose an architecture for the future application, so the commands are as follows: 

    - for x32:
    ```bash
    .\vcpkg.exe install sqlitecpp tgbot-cpp --triplet="x86-windows-static"
    ```
    
    - for x64:
    ```bash
    .\vcpkg.exe install sqlitecpp tgbot-cpp --triplet="x64-windows-static"
    ```

  It is necessary to take into account some nuances, namely, that the installation must be started through the console and in administrator mode. You need to clone or unzip the vcpkg you downloaded in the root folder: C:/vcpkg.

- [SQLite](https://www.sqlite.org/download.html) - download SQLite. Do this if you want to view the database data through the terminal(Optional)

- [DB Browser for SQLite](https://sqlitebrowser.org/dl/) - download DB Browser for SQLite. Do this if you want to view database data through a graphical tool(Optional)

- [Python](https://www.python.org/downloads/) - download python(Optional). Download the following python packages:
  ```bash
  pip install pywin32
  pip install winshell
  ```
  Also, don't forget to run the following command: python -m pip install --upgrade pip.

- When building the project, do not use paths to the project with directory names of another language, it is best to use paths with English directory names, because if this is not done, there will be problems when building the project. Also, don't use project paths with directory names that contain spaces. Also, after installing all the packages, I would advise you to restart the computer.

#### Linux:

- Since different Linux distributions have different package managers, you will have to manually search for package names and install them for your distribution

- Before starting to install the packages, do not forget to update the system. And the main packages must also be installed: build-essential and pkg-config

- download WinRar or 7-Zip(WinRar or 7-Zip or Git)

- download git(WinRar or 7-Zip or Git)

- download cmake, the minimum version you should download: 3.22.1

- download make

- download compiler: gcc(c, c++)

- download curl

- download vcpkg (using git or go to https://github.com/Microsoft/vcpkg.git to download the rar or zip file, you can also use the package manager), then you need to run the initial script to create vcpkg(.\vcpkg\bootstrap-vcpkg.bat). Next, you will need to install certain packages, namely: sqlitecpp and tgbot-cpp, as well as choose an architecture for the future application, so the commands are as follows: 

    - for x32:
    ```bash
    ./vcpkg install sqlitecpp tgbot-cpp --triplet="x86-linux"
    ```
    
    - for x64:
    ```bash
    ./vcpkg install sqlitecpp tgbot-cpp --triplet="x64-linux"
    ```

  It is necessary to take into account some nuances, namely, that the installation must be started through the console and in administrator mode. You need to clone or unzip the vcpkg you downloaded in the root folder: /vcpkg.

- download SQLite. Do this if you want to view the database data through the terminal(Optional)

- download DB Browser for SQLite. Do this if you want to view database data through a graphical tool(Optional)

- download python(Optional). Also, don't forget to run the following command: python -m pip install --upgrade pip.

- When building the project, do not use paths to the project with directory names of another language, it is best to use paths with English directory names, because if this is not done, there will be problems when building the project. Also, don't use project paths with directory names that contain spaces. Also, after installing all the packages, I would advise you to restart the computer.
