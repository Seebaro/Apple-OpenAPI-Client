# AccessibilityDeclarationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AccessibilityDeclaration]**](AccessibilityDeclaration.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.accessibility_declarations_response import AccessibilityDeclarationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationsResponse from a JSON string
accessibility_declarations_response_instance = AccessibilityDeclarationsResponse.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationsResponse.to_json())

# convert the object into a dict
accessibility_declarations_response_dict = accessibility_declarations_response_instance.to_dict()
# create an instance of AccessibilityDeclarationsResponse from a dict
accessibility_declarations_response_from_dict = AccessibilityDeclarationsResponse.from_dict(accessibility_declarations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


