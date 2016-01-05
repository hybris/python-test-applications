# Python Test Applications

A collection of applications used for testing the Python buildpack

## Applications

| Name | Description
| ---- | -----------
| `flask-application` | An application using [Flask](http://flask.pocoo.org/) microframework

### Output Content

All applications support the following REST operations:

| URI | Description
| --- | -----------
| `GET /` | The health of the application

## Building

Before building the project, the following tools must be installed:

* [Python](https://nodejs.org/en/download/)
* [Pip](https://pip.pypa.io/en/stable/installing/)

To build the project, navigate to the app directory and run the following:

```
pip install -r requirements.txt
```

## Deploying to Cloud Foundry

Each test application contains a `manifest.yml` file which allows the built application to be deployed to Cloud Foundry by simply issuing:

```
cf push
```
