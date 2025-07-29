# AccessibilityDeclarationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AccessibilityDeclarationCreateRequestDataAttributes**](AccessibilityDeclarationCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.accessibility_declaration_create_request_data import AccessibilityDeclarationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationCreateRequestData from a JSON string
accessibility_declaration_create_request_data_instance = AccessibilityDeclarationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationCreateRequestData.to_json())

# convert the object into a dict
accessibility_declaration_create_request_data_dict = accessibility_declaration_create_request_data_instance.to_dict()
# create an instance of AccessibilityDeclarationCreateRequestData from a dict
accessibility_declaration_create_request_data_from_dict = AccessibilityDeclarationCreateRequestData.from_dict(accessibility_declaration_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


