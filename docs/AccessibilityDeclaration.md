# AccessibilityDeclaration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AccessibilityDeclarationAttributes**](AccessibilityDeclarationAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.accessibility_declaration import AccessibilityDeclaration

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclaration from a JSON string
accessibility_declaration_instance = AccessibilityDeclaration.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclaration.to_json())

# convert the object into a dict
accessibility_declaration_dict = accessibility_declaration_instance.to_dict()
# create an instance of AccessibilityDeclaration from a dict
accessibility_declaration_from_dict = AccessibilityDeclaration.from_dict(accessibility_declaration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


