# AccessibilityDeclarationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestData**](AccessibilityDeclarationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.accessibility_declaration_create_request import AccessibilityDeclarationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationCreateRequest from a JSON string
accessibility_declaration_create_request_instance = AccessibilityDeclarationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationCreateRequest.to_json())

# convert the object into a dict
accessibility_declaration_create_request_dict = accessibility_declaration_create_request_instance.to_dict()
# create an instance of AccessibilityDeclarationCreateRequest from a dict
accessibility_declaration_create_request_from_dict = AccessibilityDeclarationCreateRequest.from_dict(accessibility_declaration_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


