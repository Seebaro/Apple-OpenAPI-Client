# DiagnosticSignatureRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**logs** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_signature_relationships import DiagnosticSignatureRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticSignatureRelationships from a JSON string
diagnostic_signature_relationships_instance = DiagnosticSignatureRelationships.from_json(json)
# print the JSON string representation of the object
print(DiagnosticSignatureRelationships.to_json())

# convert the object into a dict
diagnostic_signature_relationships_dict = diagnostic_signature_relationships_instance.to_dict()
# create an instance of DiagnosticSignatureRelationships from a dict
diagnostic_signature_relationships_from_dict = DiagnosticSignatureRelationships.from_dict(diagnostic_signature_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


