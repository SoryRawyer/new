### new — create a new project

Create a new project by doing the following:
- create project directory
- initialize git repo
- initialize certain dependency-management things:
  - golang: [dep](https://github.com/golang/dep)
  - python: [pipenv](https://github.com/pypa/pipenv)

Basically a bad ripoff of Rust's ```cargo init```

Example usage:
```$ new python fdsa```

Creates:
```sh
$ tree -a fdsa -L 1
fdsa
├── .git
├── .gitignore
└── Pipfile
```

```$ new golang scratch```

Creates:
```sh
$ tree -a scratch/ -L 1
scratch/
├── .git
├── .gitignore
├── Gopkg.lock
├── Gopkg.toml
└── vendor
```

#### Dependencies
git, pipenv, dep
Golang projects *must* be created in the GOPATH
