# DiagnosticSignature


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**DiagnosticSignatureAttributes**](DiagnosticSignatureAttributes.md) |  | [optional] 
**relationships** | [**DiagnosticSignatureRelationships**](DiagnosticSignatureRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.diagnostic_signature import DiagnosticSignature

# TODO update the JSON string below
json = "{}"
# create an instance of DiagnosticSignature from a JSON string
diagnostic_signature_instance = DiagnosticSignature.from_json(json)
# print the JSON string representation of the object
print(DiagnosticSignature.to_json())

# convert the object into a dict
diagnostic_signature_dict = diagnostic_signature_instance.to_dict()
# create an instance of DiagnosticSignature from a dict
diagnostic_signature_from_dict = DiagnosticSignature.from_dict(diagnostic_signature_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


