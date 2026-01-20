# BCI-Wiki-POC

# Install

Create a python virtual environment (venv) and activate it 

```
python3 -m venv .venv
source .venv/bin/activate
```

Install pip, setuptools and wheel into the venv

```
python -m pip install --upgrade pip setuptools wheel
```

Install the following packages 

```
pip install mkdocs-static-i18n

pip install mkdocs

```

```
pip install mkdocs-awesome-nav
mkdocs-redirects
```

# Running

To serve the page locally for development purposes, run the following command after completing the installation section above

```
mkdocs serve --watch-theme
```

This command will serve the website locally and reload when changes are detected. the --watch-theme flag is required as the default command will not reload the page when the custom template is modified.


# Theme Customization


# Localization support

Localization support is enabled for this mkdocs instance. Each language you wish to support should have its respective directory with files. 

```
docs
├── assets
│   └── image_non_localized.png
├── en
│   ├── image.png
│   ├── index.md
│   ├── topic1
│   │   └── index.md
│   └── topic2
│       └── index.md
└── fr
    ├── image.png
    ├── index.md
    ├── topic1
    │   └── index.md
    └── topic2
        └── index.md
