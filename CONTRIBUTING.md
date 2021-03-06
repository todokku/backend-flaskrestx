# Contributing

Contributions are **welcome** and will be fully **credited**. This page details how to 
contribute and the expected code quality for all contributions.

## Pull Requests

We accept contributions via Pull Requests.

- **Add tests!** - Your patch won't be accepted if it doesn't have tests. We follow TDD patterns, 
so code coverage need to be ~100%. Continuous Integrations are enabled, so your PR need to pass them before accepted. See instructions below.

- **Document any change in behaviour** - Make sure the `README.md` and any other relevant documentation are kept up-to-date.

- **Consider our release cycle** - We try to follow [SemVer v2.0.0](http://semver.org/). Randomly breaking public APIs is not an option.

- **Create feature branches** - Don't ask us to pull from your master branch.

   - Create a branch `feature-myawesomefeature` or `hotfix-myhotfix` from `develop`
   - Push your branch against `develop` branch.

- **One pull request per feature** - If you want to do more than one thing, send multiple pull requests.

- **Send coherent history** - Make sure each individual commit in your pull request is meaningful. If you had to make multiple intermediate commits while developing, please [squash them](http://www.git-scm.com/book/en/v2/Git-Tools-Rewriting-History#Changing-Multiple-Commit-Messages) before submitting.


## Running Tests

``` bash
(env) $ python -m pytest "project/tests" --cov="project"
(env) $ python -m black project
(env) $ python -m flake8 project
(env) $ python -m isort project/**/*.py
```

You can also run
``` bash
$ docker-compose exec app python -m pytest "project/tests" --cov="project"
$ docker-compose exec app python -m black project
$ docker-compose exec app python -m flake8 project
$ docker-compose exec app python -m isort project/**/*.py
```

**Happy coding**!