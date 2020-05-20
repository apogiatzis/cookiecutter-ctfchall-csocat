# CTF Challenge C Socat Template
Cookiecutter template for generating a basic skeleton directory structure and files to develop a C-based ctf challenge that allows remote multiple connections using socat. The template is accompanied with the relevant docker files such that build and execution are performed in an isolated environment. 

That being said, apart from cookiecutter docker is a required dependency to build and run the challenge.

## Get Started

### Dependencies
Make sure docker and cookiecutter are installed in your system.

You can install docker by following the intructions in the official website [here](https://docs.docker.com/get-docker/).

Cookiecutter can be simply installed by running:
```
pip install cookiecutter
```

### Create template 
To create a challenge template run:
```
cookiecutter https://github.com/apogiatzis/cookiecutter-ctfchall-csocat
```