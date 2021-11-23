
### Purpose
Show the complete source code of a filter/transformer or connector including all transformer steps and optionally also all includes (currently only for connectors).
### Structure
`var sourceCode = getSourceCode(showEverything, hideThis);`
### Parameters

| Parameter  | Description | Default Value |
| ------------- | ------------- | ------------- |
| **showEverything**  | If this flag is set to true, it will not just show the code of the transformers but also the imported code (like code templates, maps, etc.) This flag currently only works for connectors and will be ignored for transformers | _false_ |
|**hideThis**|If this flag is set to true, this function and also it's call will be hidden from the source code.|_true_|
|**return value**|The formated javascript sourcecode as string|-|

### Usage
Add a line of code like this: `logger.info(getSourceCode(true));` to your transformer.
