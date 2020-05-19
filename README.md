# latex-completion-data

An automatically generated data set that can be used to provide code completion for the LaTeX typesetting system.
It is used by the [TexLab](https://texlab.netlify.com/) language server.

## Development

We use [Docker](https://www.docker.com/) to ensure reproducible builds.
A new data set can be generated by executing

```sh
docker build --tag=latex-completion-data --no-cache .
docker run --name latex-completion-data -t latex-completion-data
docker cp latex-completion-data:/app/latex-completion-data/completion.json .
```
