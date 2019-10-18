# InterSystems-Template
This is a template for an InterSystems ObjectScript Github repository.
The template goes also with a few files which let you immedietly compile your ObjecScript files in InterSystems IRIS Community Edition in a docker container

## Prerequisites
This needs to have git and docker installed.

## Installation 
Clone/git pull the repo into any local directory

```
$ git clone https://github.com/ruperez/intersystems-template.git
```

Open the terminal in this directory and run:

```
$ docker-compose build
```

3. Run the IRIS container with your project:

```
$ docker-compose up -d
```

## How to Test it

Open an IRIS terminal:

```
$ docker-compose exec iris iris session iris
USER>write ##class(PackageSample.ObjectScript).Test()
```

### .vscode/settings.json
Settings file to let you immedietly code in VSCode

### .vscode/launch.json
Config file if you want to debug with VSCode ObjectScript
