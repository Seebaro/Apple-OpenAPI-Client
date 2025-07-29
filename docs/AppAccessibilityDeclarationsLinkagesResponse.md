# AppAccessibilityDeclarationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppAccessibilityDeclarationsLinkagesResponseDataInner]**](AppAccessibilityDeclarationsLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_accessibility_declarations_linkages_response import AppAccessibilityDeclarationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAccessibilityDeclarationsLinkagesResponse from a JSON string
app_accessibility_declarations_linkages_response_instance = AppAccessibilityDeclarationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAccessibilityDeclarationsLinkagesResponse.to_json())

# convert the object into a dict
app_accessibility_declarations_linkages_response_dict = app_accessibility_declarations_linkages_response_instance.to_dict()
# create an instance of AppAccessibilityDeclarationsLinkagesResponse from a dict
app_accessibility_declarations_linkages_response_from_dict = AppAccessibilityDeclarationsLinkagesResponse.from_dict(app_accessibility_declarations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


