# AppAppInfosLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppInfoLocalizationRelationshipsAppInfoData]**](AppInfoLocalizationRelationshipsAppInfoData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_infos_linkages_response import AppAppInfosLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppInfosLinkagesResponse from a JSON string
app_app_infos_linkages_response_instance = AppAppInfosLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppInfosLinkagesResponse.to_json())

# convert the object into a dict
app_app_infos_linkages_response_dict = app_app_infos_linkages_response_instance.to_dict()
# create an instance of AppAppInfosLinkagesResponse from a dict
app_app_infos_linkages_response_from_dict = AppAppInfosLinkagesResponse.from_dict(app_app_infos_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


