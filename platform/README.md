# Platform

This folder contains the **platform**.
It includes everything needed to develop the platform itself as well as its sample applications.
The platform serves as a central location for all files that are generic and intended to be reused by product development teams.
These include for example Zephyr modules, scripts, and the Docker-based build environment.

The platform is developed alongside the pilot projects within the monorepo.
Later, it can be extracted into a standalone repository (e.g., via Copybara) so that other projects can include it using Git submodules or `git-subrepo`.

**Note:** Because the platform also contains the build environment (Docker) and supporting scripts required by product projects to start the development environment (e.g., to run `west`), it cannot be integrated as a west project.

