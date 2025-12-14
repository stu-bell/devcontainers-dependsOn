This devcontainer config adds a local feature that uses the dependsOn property to require a dependency feature to be installed, before the feature specified in the devcontainer.json is installed. 

The demo feature is defined locally in .devcontainer/features/dependsOnDemo and lists ghcr.io/devcontainers/feature-starter/hello:latest as a dependency, which installs a demo command `hello`.

When the devcontainer is started, the command `hello` should be available inside the devcontainer.

To test, open this repo in GitHub codespaces and run the command `hello`

Spec: https://containers.dev/implementors/features/#dependsOn

