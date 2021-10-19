# Data Science Dev Environment
This is a starter data science docker dev environment.

[![Open In Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/ANRGUSC/data_science_workspace)

The Dev environment comes with R, Python 3.8, and many of the standard 
data science python packages pre-installed (see the 
[requirements.txt](./requirements.txt) file).
You can fork this repository and modify the files for you needs!

## Usage
You can open the dev environment in GitPod by clicking the "Open in GitPod Button at the top of this README, or open on your system with VSCode by cloning this repository, opening it with VSCode, and then using the Remote Development extension to "Reopen in Container".

## Documentation
There are two sets of config files in this repo: one for local development and the other for development on Gitpod. 
Both use the same dockerfile to specify the dev environment, but since each executes on a different platform (the first via VSCode and Docker installed on your machine and the second on Gitpod's cloud servers) their settings are specified through seperate configuration files. 

### Local Development
All config files for local development can be found in the [./.devcontainer](./.devcontainer) directory. 
There are two files: [devcontainer.json](./.devcontainer/devcontainer.json) and [Dockerfile](./.devcontainer/Dockerfile).
The devcontainer.json file contains information like the name of the dev container, its context, the dockerfile its based on, settings, VSCode extensions to install in the container, commands to run once the container has been created, etc. 
There are many settings you can change here to customize your environment.
See the documentation [here](https://code.visualstudio.com/docs/remote/devcontainerjson-reference) for a comprehensive list of all settings.

### Gitpod  Development
We've setup the Gitpod environment to use the same Dockerfile as is used in the local dev environment to make things as consistent as possible. 
Gitpod, however, uses the [.gitpod.yml](./.gitpod.yml) file rather than the devcontainer.json file to configure settings, extenstions, commands, etc. 
Visit the docs [here](https://www.gitpod.io/docs/configure) for a comprehesive list of all confuration options!
Also, checkout our internal gitpod docs/tips/tricks repo [here](https://github.com/ANRGUSC/gitpod) for tips on customization.