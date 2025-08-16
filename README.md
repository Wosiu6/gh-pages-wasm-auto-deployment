# WASM Github Pages Deployment
This is a repo that documents how to publish a WASM generated Blazor Server page to Github Pages

## Setup
- Copy .nojekyll file to your git root
- Go to your repo Settings -> Actions -> General -> Workflow permissions, grant Read and write permissions to the GITHUB_TOKEN when running workflows in this repo.
- Go to Actions -> New workflow -> set up a workflow yourself, copy contents of main.yaml into the editor
- Replace NAME.sln with your Blazor WASM solution file name
- Commit changes

- Depending on your .NET version you might have to change that as well

## WASM .NET6
If you are using .NET6 WASM, use the main_net6.yml version instead, as it will install wasm-tools-net6 which are required to run wasm build.