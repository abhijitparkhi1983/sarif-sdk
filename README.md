# sarif-sdk
The SARIF SDK contains .NET code and supporting files for working with the Static Analysis Results Interchange Format (SARIF). For more information about SARIF, see the [SARIF Home Page](http://sarifweb.azurewebsites.net). You can read the [SARIF specification](https://rawgit.com/sarif-standard/sarif-spec/master/Static%20Analysis%20Results%20Interchange%20Format%20(SARIF).html), or file [issues](https://github.com/sarif-standard/sarif-spec/issues) in the [SARIF GitHub repo](https://github.com/sarif-standard/sarif-spec).

## Getting started

To add the SARIF SDK to your project, install the Sarif.Sdk [NuGet package](https://www.nuget.org/packages/Sarif.Sdk). Sarif.Sdk depends on [Newtonsoft.Json](http://www.newtonsoft.com/json), which is installed automatically when you install Sarif.Sdk.

The types in the SARIF SDK are in the `Microsoft.CodeAnalysis.Sarif` namespace.

The SARIF SDK provides a set of classes which represent the elements of the SARIF format. We refer to this as the "SARIF object model". The root type that represents a SARIF log file is `SarifLog`. Other types in the SARIF object model are `Result`, `PhysicalLocation`, _etc._.

Note: The SARIF SDK's build process automatically generates the SARIF object model classes from the SARIF JSON schema, which you can find at [`src/Sarif/Schemata/Sarif.schema.json`](https://github.com/Microsoft/sarif-sdk/blob/master/src/Sarif/Schemata/Sarif.schema.json). So you won't find the source code for these classes in the repo.

In addition to the object model, the SARIF SDK provides a set of helper classes to facilitate using Newtonsoft.Json to read and write SARIF log files.

## Accomplishing common tasks

To learn how to accomplish common tasks with the SARIF SDK, such as reading and writing files from disk,
see the [How To](https://github.com/Microsoft/sarif-sdk/blob/master/docs/how-to.md) page.
