# AccessibilityDeclarationUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationUpdateRequestData**](AccessibilityDeclarationUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.accessibility_declaration_update_request import AccessibilityDeclarationUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationUpdateRequest from a JSON string
accessibility_declaration_update_request_instance = AccessibilityDeclarationUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationUpdateRequest.to_json())

# convert the object into a dict
accessibility_declaration_update_request_dict = accessibility_declaration_update_request_instance.to_dict()
# create an instance of AccessibilityDeclarationUpdateRequest from a dict
accessibility_declaration_update_request_from_dict = AccessibilityDeclarationUpdateRequest.from_dict(accessibility_declaration_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


