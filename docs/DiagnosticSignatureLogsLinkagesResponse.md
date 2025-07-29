# DiagnosticSignatureLogsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DiagnosticSignatureLogsLinkagesResponseDataInner]**](DiagnosticSignatureLogsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_signature_logs_linkages_response import DiagnosticSignatureLogsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticSignatureLogsLinkagesResponse from a JSON string
diagnostic_signature_logs_linkages_response_instance = DiagnosticSignatureLogsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(DiagnosticSignatureLogsLinkagesResponse.to_json())

# convert the object into a dict
diagnostic_signature_logs_linkages_response_dict = diagnostic_signature_logs_linkages_response_instance.to_dict()
# create an instance of DiagnosticSignatureLogsLinkagesResponse from a dict
diagnostic_signature_logs_linkages_response_from_dict = DiagnosticSignatureLogsLinkagesResponse.from_dict(diagnostic_signature_logs_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


