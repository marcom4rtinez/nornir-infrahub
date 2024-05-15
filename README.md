<!-- markdownlint-disable -->
![Infrahub Logo](https://assets-global.website-files.com/657aff4a26dd8afbab24944b/657b0e0678f7fd35ce130776_Logo%20INFRAHUB.svg)
<!-- markdownlint-restore -->

# Infrahub by OpsMill

[Infrahub](https://github.com/opsmill/infrahub) by [OpsMill](https://opsmill.com) acts as a central hub to manage all of the information and code that powers your infrastructure. At its heart, Infrahub is built on 3 fundamental pillars:

- **A Flexible Schema**: A model of the infrastructure and the relation between the objects in the model, that's easily extensible.
- **Version Control**: Natively integrated into the graph database which opens up some new capabilities like branching, diffing, and merging data directly in the database.
- **Unified Storage**: By combining a graph database and git, Infrahub stores data and code needed to manage the infrastructure.

## [Nornir](https://github.com/nornir-automation/nornir) plugin for [Infrahub](https://github.com/opsmill/infrahub)

### Installation

```bash
pip install nornir_infrahub
```

### Infrahub as the Nornir inventory

Infrahub can be used as an inventory source for Nornir.
An example of this can be found in [./examples/nornir_inventory.py](./examples/nornir_inventory.py)

### Infrahub Artifact Tasks

A set of tasks are provided to operate on Infrahub Artifacts:

- `generate_artifacts`: generates the Artifacts for a Artifact Definition
- `regenerate_artifact`: re-generates an Artifact for a Nornir Host
- `get_artifact`: retrieve an Artifact for a Nornir Host

An example of this can be found in [./examples/nornir_tasks.py](./examples/nornir_tasks.py)
