# Instructions for developers
See [wiki](https://github.com/vijayvarma392/gw_eccentricity/wiki).

## Contributing to gw_eccentricity

The preferred method of making contributions is to
[fork](https://help.github.com/articles/fork-a-repo/) + [pull
request](https://help.github.com/articles/about-pull-requests/) from the main
[repo](https://github.com/vijayvarma392/gw_eccentricity).

Before doing a pull request, you should check that your changes don't break
anything by running the following from the root directory of your check-out.
Every pull request will be automatically tested by github.
```
./run_tests
```

## Adding a new eccentricity definition
For adding a new definition of eccentricity follow the guidelines [here](https://github.com/vijayvarma392/gw_eccentricity/wiki/Adding-new-eccentricity-definitions)

## Waveform data
Follow the instructions in `data/README.md`

## PyPI release
Note: This is currently under Vijay's account, so only he can do this.
```shell
python setup.py sdist bdist_wheel
twine upload dist/*
```
