# AccessibilityDeclarationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AccessibilityDeclarationUpdateRequestDataAttributes**](AccessibilityDeclarationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.accessibility_declaration_update_request_data import AccessibilityDeclarationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationUpdateRequestData from a JSON string
accessibility_declaration_update_request_data_instance = AccessibilityDeclarationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationUpdateRequestData.to_json())

# convert the object into a dict
accessibility_declaration_update_request_data_dict = accessibility_declaration_update_request_data_instance.to_dict()
# create an instance of AccessibilityDeclarationUpdateRequestData from a dict
accessibility_declaration_update_request_data_from_dict = AccessibilityDeclarationUpdateRequestData.from_dict(accessibility_declaration_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


