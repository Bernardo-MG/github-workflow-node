# Github Workflow Files for Node

Github workflow files for using CI in Node projects.

## Features

- SSH deployment

## Usage

Use these files as any reusable workflow:

```
jobs:
  tests:
    name: Tests with JDK ${{ matrix.jdk }}
    strategy:
      matrix:
        jdk: [ 11, 17 ]
    uses: Bernardo-MG/github-workflow-maven/.github/workflows/testing.yml@v1
    with:
      jdk: ${{ matrix.jdk }}
```

For an actual usage of these files check the [Library Maven Archetype][archetype].

## Collaborate

Any kind of help with the project will be well received, and there are two main ways to give such help:

- Reporting errors and asking for extensions through the issues management
- or forking the repository and extending the project

### Issues management

Issues are managed at the GitHub [project issues tracker][issues], where any Github user may report bugs or ask for new features.

### Getting the code

If you wish to fork or modify the code, visit the [GitHub project page][scm], where the latest versions are always kept. Check the 'master' branch for the latest release, and the 'develop' for the current, and stable, development version.

## License

The project has been released under version 2.0 of the [Apache License][license].

[archetype]: https://github.com/Bernardo-MG/library-maven-archetype
[issues]: https://github.com/Bernardo-MG/github-workflow-maven/issues
[license]: https://www.apache.org/licenses/LICENSE-2.0
[scm]: https://github.com/Bernardo-MG/github-workflow-maven
