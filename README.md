# Flask

**Flask** is a Python [micro framework](https://flask.palletsprojects.com/en/3.0.x/) for building web applications.

# Demo Application

## Prerequisite

A working terminal running a shell is required.

To begin please install the [`Azure CLI`](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli
).

```shell
az login
az config set defaults.location=germanywestcentral
```

## Deploy to Azure

Please read the according documentation [on the Azure CLI](https://learn.microsoft.com/de-de/cli/azure/webapp?view=azure-cli-latest) and [on python apps](https://learn.microsoft.com/en-us/azure/app-service/quickstart-python) first!

```shell
az webapp up --location germanywestcentral --name my-training-flask --runtime PYTHON:3.11 --sku B1 --only-show-errors
```

Note: `name` needs to be __unique__ Azure-wide!

### Example Output

```json
{
  "URL": "http://my-training-flask.azurewebsites.net",
  "appserviceplan": "office_asp_3158",
  "location": "germanywestcentral",
  "name": "my-training-flask",
  "os": "Linux",
  "resourcegroup": "office_rg_5180",
  "runtime_version": "PYTHON|3.11",
  "runtime_version_detected": "-",
  "sku": "BASIC",
  "src_path": "//Users//gretel//cbwham//training-flask"
}
```

# Work in progress - to be continued!
