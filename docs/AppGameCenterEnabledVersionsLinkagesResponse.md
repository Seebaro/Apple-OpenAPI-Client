# AppGameCenterEnabledVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsGameCenterEnabledVersionsDataInner]**](AppRelationshipsGameCenterEnabledVersionsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_game_center_enabled_versions_linkages_response import AppGameCenterEnabledVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppGameCenterEnabledVersionsLinkagesResponse from a JSON string
app_game_center_enabled_versions_linkages_response_instance = AppGameCenterEnabledVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppGameCenterEnabledVersionsLinkagesResponse.to_json())

# convert the object into a dict
app_game_center_enabled_versions_linkages_response_dict = app_game_center_enabled_versions_linkages_response_instance.to_dict()
# create an instance of AppGameCenterEnabledVersionsLinkagesResponse from a dict
app_game_center_enabled_versions_linkages_response_from_dict = AppGameCenterEnabledVersionsLinkagesResponse.from_dict(app_game_center_enabled_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


