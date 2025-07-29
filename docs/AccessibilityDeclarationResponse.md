# AccessibilityDeclarationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclaration**](AccessibilityDeclaration.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.accessibility_declaration_response import AccessibilityDeclarationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationResponse from a JSON string
accessibility_declaration_response_instance = AccessibilityDeclarationResponse.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationResponse.to_json())

# convert the object into a dict
accessibility_declaration_response_dict = accessibility_declaration_response_instance.to_dict()
# create an instance of AccessibilityDeclarationResponse from a dict
accessibility_declaration_response_from_dict = AccessibilityDeclarationResponse.from_dict(accessibility_declaration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


