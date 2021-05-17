# Upload to extrality pypi

The following commands will do that for you.
`twine` doesn't read `.netrc` and will ask your username/password.

```sh
python setup.py sdist
pip install twine
twine upload \
	--skip-existing \
	--repository-url https://pypi.extrality.ai/simple/ \
	dist/*
```
