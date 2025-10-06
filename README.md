# Zephyr Monorepo Example

This repository provides an example structure for a Zephyr-based monorepo.

In this setup, a Zephyr *platform* is developed together with one or more *pilot projects* (products).

The monorepo typically contains at least two main components:
1. **Platform** – the shared Zephyr platform with drivers, boards, subsystems, build environment, and tooling.
2. **Product (Application)** – one or more applications built on top of the platform.
3. *(Optional)* Additional products or applications.

## Notes

- Some product teams may prefer not to work directly in the monorepo. In such cases, the platform can later be extracted into its own repository (e.g. via Copybara). Other projects can then integrate the platform repository via Git submodules or `git-subrepo`.

- Since the platform also includes the build environment (Docker) and supporting scripts required by product projects (e.g. to run `west`), it cannot be integrated as a west project.

