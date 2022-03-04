# integrator-recipes

Recipes for [SprykerSdk.Integrator](https://github.com/spryker-sdk/integrator) tool.

They contain machine-readable instructions on how to integrate
core module updates into project level.
This aims to help automating the process.

## Adding recipes

Any vendor based module can have recipes here.
The structure looks as follows:
```
Spryker/                                      <- Vendor namespace
    Availability/                             <- Module name
        9.10.0/                               <- Module version
            installer-manifest.json           <- Manifest file
SprykerShop/
    CartPage/
        3.29.0/
            installer-manifest.json
.....
```

Only released versions can be added. So please make sure you only add/merge recipes after their module release has been done.

Note: If your vendor namespace is a combination (`MyCompany\MyOtherNamespace`) or alike, the backslash needs to be printed as underscore (`MyCompany_MyOtherNamespace`). We do not yet support this in the integrator tooling, but if you have such a use case please reach out and we can talk about fast-tracking this feature for it.
