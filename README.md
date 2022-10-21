# README for this repository

This repository is for landing pages on 
[the GitHub pages of hpcuantwerpen](https://hpcuantwerpen.github.io).

Linked sites:
-   [Documentation EasyBuild repository for the 2022 new module system](https://hpcuantwerpen.github.io/UAntwerpen-easybuild)
-   [Technical documentation for the 2022 new module system](https://hpcuantwerpen.github.io/UAntwerpen-modules)

## Instructions for mkdocs

These pages are rendered via [MkDocs](https://www.mkdocs.org/),
which makes it very easy to preview the result of the changes you make locally.

-   First, install ``mkdocs``, including the `material` theme and additional plugins.
    It is best to do so in a virtual environment.

    ``` bash
    python3 -m venv python3-mkdocs
    source python3-mkdocs/bin/activate
    pip install mkdocs mkdocs-material mkdocs-git-revision-date-localized-plugin
    ```

-   Start the MkDocs built-in dev-server to preview the tutorial as you work on it:

    ``` bash
    make preview
    ```

    or

    ``` bash
    mkdocs serve
    ```

  Visit http://127.0.0.1:8000 to see the local live preview of the changes you make.

* If you prefer building a static preview you can use ``make`` or ``mkdocs build``,
  which should result in a ``site/`` subdirectory that contains the rendered documentation.


