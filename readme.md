# Github Workflow Files for Node

Github workflow files for using CI in Node projects.

## Features

- SSH deployment

## Usage

Use these files as any reusable workflow:

```
jobs:
  deploy:
    uses: Bernardo-MG/github-workflow-node/.github/workflows/deploy_ssh.yml@v1
    with:
      branch: develop
      environment: deployment_site
    secrets:
      host: ${{ secrets.DEPLOY_HOST }}
      port: ${{ secrets.DEPLOY_PORT }}
      path: ${{ secrets.DEPLOY_PATH }}
      username: ${{ secrets.DEPLOY_USER }}
      password: ${{ secrets.DEPLOY_PASSWORD }}
```

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

[issues]: https://github.com/Bernardo-MG/github-workflow-maven/issues
[license]: https://www.apache.org/licenses/LICENSE-2.0
[scm]: https://github.com/Bernardo-MG/github-workflow-maven
