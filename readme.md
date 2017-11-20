# Autorest DotnetCore Container 
> see https://aka.ms/autorest 

## Getting Started 
To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:
> `autorest readme.md`

To see additional help and options, run:
> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration 
The following are the settings for this using this API with AutoRest.

``` yaml
# specify the version of Autorest to use
#version: 1.0.1-20170402 

namespace: Api.Client
output-folder: .
input-file: swagger.json

csharp: # just having a 'csharp' node enables the use of the csharp generator.
  output-folder : generated/csharp # relative to the global value.
  enable-xml: true
  azure-arm: true # 'azure-arm' is a declaration that the OpenAPI is an Azure arm resource (not specified as part of the generator name.)
  add-credentials: true # generates `Credentials` property
```

