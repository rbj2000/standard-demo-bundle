# Standard Demo Bundle
This is a dump using [entando-bundle-cli](https://github.com/entando-k8s/entando-bundle-cli) and the following environment:

### env.json
```
{
    "coreBaseApi": "http://quickstart-sales-demo.lab.entando.org/entando-de-app",
    "k8ssvcApi": "http://quickstart-eci-sales-demo.lab.entando.org/k8s",
    "clientId": "entando-bundle-cli",
    "clientSecret": "<insert_secret_here>"
}
```

### Dump Command:
```
$ entando-bundle from-env \
    --env env.json \
    --code standard-demo-bundle \
    --description "Standard Demo Bundle"
```

or use the interactive command to following the cli interactive version:
```
$ entando-bundle
? What do you want to do? Create a new bundle using components from an environment
? Please select an env.json file with the environment variables: env.json
? Which type of components do you want to add to the bundle? All components
Collecting all components from the provided environment...
Collecting widgets
Collecting pageModels
Collecting fragments
Collecting pages
Collecting contentTypes
Collecting contentModels
Collecting plugins
? Do you want to generate the Bundle with the selected components? Yes
? Where do you want to generate the Bundle? ./
? What's the code for the Bundle? standard-demo-bundle
? Please add a description to the Bundle: Standard Demo Bundle
Generating bundle...
```

### Disclaimer:
This hasn't been properly tested on Entando Component Manager (ECR), so please use the issues section to report ECR installation issues or changes required on `entando-bundle-cli` to support other components or formats for a full Getting Started Experience (Standard Demo).
