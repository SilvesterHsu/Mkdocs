## Outline
* Mkdocs initialization
* git initialization
* GitHub tocken

## Mkdocs initialization
Getting started is super easy.
```
mkdocs new my-project
cd my-project
```

There's a single configuration file named `mkdocs.yml`, and a folder named `docs` that will contain your documentation source files. Right now the `docs` folder just contains a single documentation page, named `index.md`.
![Git-Build-03](img/Git-Build-03.png)

> You can also start serve in the following steps:

MkDocs comes with a built-in dev-server that lets you preview your documentation as you work on it. Make sure you're in the same directory as the `mkdocs.yml` configuration file, and then start the server by running the `mkdocs serve` command:

```
$ mkdocs serve
INFO    -  Building documentation...
INFO    -  Cleaning site directory
[I 160402 15:50:43 server:271] Serving on http://127.0.0.1:8000
[I 160402 15:50:43 handlers:58] Start watching changes
[I 160402 15:50:43 handlers:60] Start detecting changes
```
Open up `http://127.0.0.1:8000/` in your browser, and you'll see the default home page being displayed:
![Git-Build-04](img/Git-Build-04.png)

> You could also use `mkdocs serve -a <yourhost>:<port>` to specify the serve.

Example:
```
$ mkdocs serve -a 0.0.0.0:8000
INFO    -  Building documentation...
INFO    -  Cleaning site directory
[I 190414 02:43:38 server:298] Serving on http://0.0.0.0:8000
[I 190414 02:43:38 handlers:59] Start watching changes
[I 190414 02:43:38 handlers:61] Start detecting changes
```

## Git Initialization
Enter `<your project>` folder through the terminal.
```
git init
git add .
git commit -m "Basic Mkdocs files"
```
## GitHub Tocken
We need `GITHUB_TOKEN` for Travis to build Mkdocs. So we generate one in [Personal access tokens](https://github.com/settings/tokens).(or you can go `Settings -> Developer settings -> Personal access tokens` to generate one).

![Git-Build-01](img/Git-Build-01.jpg)

And make sure click every selection.

![Git-Build-02](img/Git-Build-02.png)

Copy the token we generated for later use.
