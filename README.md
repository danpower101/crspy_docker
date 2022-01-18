# crspy_docker
A dockerized dev container for crspy (work in progress so **keep backups** - will update detailed instructions shortly)

# Requirements
This works with vscode only (https://code.visualstudio.com/docs/python/python-tutorial)

- vscode (https://code.visualstudio.com/docs/remote/containers)
- docker (https://www.docker.com/)

# Quick steps

- Clone crspy_docker
- In crspy_docker folder on your home system, add a folder which will be your working directory (e.g. `wd`)
- Open `docker-compose.yaml` for editing
- Under volumes change `/path/to/your/wd` to the system path to your newly created folder `wd` and save
- Press ctrl+shft+P and type `rebuild and reopen container` click this (it will provide a pop up when opening folder in future)
- First run will take time whilst it downloads and builds

You can now create files in the wd and run crspy as normal (e.g. check https://github.com/danpower101/crspy_example for walkthrough). Build the folder strucutre and run. Essentially crspy is now running in a virtual machine with all dependencies pre-installed. Any changes/files you add to the wd will remain on your home computer. This could help when moving between operating systems
