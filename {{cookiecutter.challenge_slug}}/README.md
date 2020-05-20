# {{cookiecutter.challenge_name}}
**Category:** {{cookiecutter.category}}

**Author:** {{cookiecutter.author}}

## Description
{{cookiecutter.description}}

## Points
{{cookiecutter.points}}

## Solution
<details>
 <summary>Reveal Spoiler</summary>

 ## Flag
`{{cookiecutter.flag}}`


</details>

## Run locally
### Build
```
docker build -t {{ cookiecutter.docker_image }} .
```

### Extract Artifacts from Container
```
CID=$(docker create {{ cookiecutter.docker_image }}) && docker cp $CID:/root/chall public/ || docker rm $CID
```

### Run
```
docker run --read-only -p {{cookiecutter.port}}:{{cookiecutter.port}} -d --restart=always {{ cookiecutter.docker_image }}
```