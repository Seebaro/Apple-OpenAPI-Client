# BuildDiagnosticSignaturesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BuildDiagnosticSignaturesLinkagesResponseDataInner]**](BuildDiagnosticSignaturesLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_diagnostic_signatures_linkages_response import BuildDiagnosticSignaturesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildDiagnosticSignaturesLinkagesResponse from a JSON string
build_diagnostic_signatures_linkages_response_instance = BuildDiagnosticSignaturesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BuildDiagnosticSignaturesLinkagesResponse.to_json())

# convert the object into a dict
build_diagnostic_signatures_linkages_response_dict = build_diagnostic_signatures_linkages_response_instance.to_dict()
# create an instance of BuildDiagnosticSignaturesLinkagesResponse from a dict
build_diagnostic_signatures_linkages_response_from_dict = BuildDiagnosticSignaturesLinkagesResponse.from_dict(build_diagnostic_signatures_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


