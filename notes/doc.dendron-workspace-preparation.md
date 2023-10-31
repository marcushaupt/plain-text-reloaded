---
id: 4agl47een0xc6ufny8txqxe
title: Dendron Workspace Preparation
desc: First steps to setup Dendron workspace for a productive environment
updated: 1698759116639
created: 1698749115909
author: Marcus Haupt
mail: marcus@haupt.contact
website: 'https://marcus.haupt.contact'
---
_Edit the [[templates.doc]] note to change this template created for Dendron Documnetation Notes._

## Preface

<!-- Describe a short summary about target of this documentation. -->

## Initialize a new Dendron workspace

<!-- Use # to structure the documentation. Always start with ## instead of # because # is reserved for the $title$ that is created by the metdata. -->

## Add remote Vaults

Adding [Dendron Vaults](https://wiki.dendron.so/#vaults) to Dendron can significantly enhance the user experience. A Vault is nothing more than a directory of files and has no encryption, as the term might imply. It is possible to include a Vault via a local or remote resource. It doesn't matter what the structure of the directory is. Also another Dendron workspace can be used as a Vault. Typically, this is a GIT repository.

To better understand the feature and I recommend to start by including the [Dendron Handbook](https://github.com/dendronhq/handbook) as a Vault in the new Workspace.

To do this, the command `Dendron: Add Existing Vault` must be rounded up. Afterwards, the selection can be used to specify whether this is a `local` or `remote` Vault. Depending on the selection, the local path or the GIT repository (SSH access must be set up) must then be specified.

Der Vault wird in der selben Verzeichnisstruktur angelegt, wie der Workspace und die Inhalte können ebenso verändert oder angepasst werden.

### Add Plain Text: Templates Vault

To use the templates for the [Plain Text: Reloaded](https://github.com/marcushaupt/plain-text-reloaded) project, I recommend opening a remote Vault for it.

To do this, execute the command `Dendron: Add Existing Vault` as already described. Then select `remote` and enter the SSH repository path `git@github.com:marcushaupt/plain-text-templates.git`. Alternatively, you can first create a fork to the [Plain Text: Templates](https://github.com/marcushaupt/plain-text-templates) repository and use your fork as a remote vault. This allows you to customize the templates to your liking.

Your workspace should now look something like this:

```bash
.
├── LICENSE
├── README.md
├── dendron.code-workspace
├── dendron.yml
├── dependencies
│   └── github.com
└── notes
    ├── root.md
    ├── root.schema.yml
```

The remote Vaults can be found here:

```bash
├── dependencies
    └── github.com
        ├── dendronhq
        │   └── handbook
        └── marcushaupt
            └── plain-text-templates
```

### Topic B.1

### Topic B.2

#### Topic B.2.1

## Ressources

- [Plain Text: Reloaded](https://github.com/marcushaupt/plain-text-reloaded)
- [Plain Text: Templates](https://github.com/marcushaupt/plain-text-templates)
- [Dendron Handbook](https://github.com/dendronhq/handbook)
- [Dendron Vaults](https://wiki.dendron.so/#vaults)
