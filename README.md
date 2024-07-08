<div align="center">
<a href="https://github.com/algorandfoundation/algokit-fullstack-template"><img src="https://bafkreiecql6vi6othgvbouvofyajmm52jyinnppaw7ckenxxeywjbwf2v4.ipfs.nftstorage.link" width=60%></a>
</div>

<p align="center">
    <a target="_blank" href="https://github.com/algorandfoundation/algokit-cli"><img src="https://img.shields.io/badge/docs-repository-00dc94?logo=github&style=flat.svg" /></a>
    <a target="_blank" href="https://developer.algorand.org/algokit/"><img src="https://img.shields.io/badge/learn-AlgoKit-00dc94?logo=algorand&mac=flat.svg" /></a>
    <a target="_blank" href="https://github.com/algorandfoundation/algokit-base-template"><img src="https://img.shields.io/github/stars/algorandfoundation/algokit-base-template?color=00dc94&logo=star&style=flat" /></a>
    <a target="_blank" href="https://developer.algorand.org/algokit/"><img  src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Falgorandfoundation%2Falgokit-base-template&countColor=%2300dc94&style=flat" /></a>
</p>

---

This base template provides a baseline structure for an empty AlgoKit workspace project.

## Structure

The base workspace project structure looks as follows:

```md
.
├── .algokit.toml # configuration file for algokit that defines this root folder as a workspace
├── projects # main folder for all sub-projects that can be added to the workspace by executing `algokit init` in the root folder
└── README.md # this file, including main instructions on navigating within the workspace
```

To use this template, [install AlgoKit](https://github.com/algorandfoundation/algokit-cli#readme) and then either execute `algokit init`. Any standalone template will auto include the content of this template as a base. To disable this behavior use the `--no-workspace` flag.

### Notes for template builders

Template contains a set of hidden questions that can be altered via explicit `-a` flag in `algokit init` command. Those are useful when base template is part of your copier `_tasks` (see [fullstack](https://github.com/algorandfoundation/algokit-fullstack-template/blob/main/copier.yaml) for reference) invocation and you want to control behavior around optional artifacts that are disabled by default.

### GitHub Codespaces

If executing this repository in GitHub Codespaces, execute `algokit generate devcontainer` to create default `.devcontainer.json` file prior to provisioning a codespace instance and commit to version control. Then, after codespace creation, the container will automatically cleanup templatized content and pre-install `algokit` for you. To get started execute:

- `algokit init` - to invoke interactive wizard to guide you through the process of creating a new AlgoKit project

Powered by [Copier templates](https://copier.readthedocs.io/en/stable/).
