# Paperbin

A collection of small forks for paper, usually intended for PR testing
or tracing.

## Project layout
The project is split into the `main` branch and `fork/*` branches.
Each `fork/*` branch represents a separate fork of paper with a separate purpose.
The project does include a submodule referencing the current paper main branch.
However, this does **NOT** need to be initialised, it only exists for automated
updates via dependabot and acts as a replacement for the paper commit reference.

## Building a fork

The project uses `paperweight-patcher`.  
It can be build by running `./gradlew applyAllPatches`, followed by `./gradlew createMojmapPaperclipJar`.  
The resulting jar can be found in `paperbin-server/build/libs/paperbin-paperclip-*-SNAPSHOT-mojmap.jar`.
