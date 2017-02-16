# Submodule

L'outils submodule permet d'inclure des projets git dans un autre projet.

## Ajouter un submodule

### Transformer un répertoire existant en submodule

    git submodule init <path>

### Importer un projet en tant que sous-projet

    git submodule add <url>

### Importer le submodule après avoir cloné

    git submodule update --init --recursive

## Webographie


---
  - id: submodule-scm-doc
    title: Git Tools - Submodules
    author: git-scm doc
    url: https://git-scm.com/book/en/v2/Git-Tools-Submodules
  - id: submodule-scm-man
    title: Submodule
    author: git-scm man pages
    url: https://git-scm.com/docs/git-submodule
...
