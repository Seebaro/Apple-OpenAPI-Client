# AppInfoAppInfoLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppInfoRelationshipsAppInfoLocalizationsDataInner]**](AppInfoRelationshipsAppInfoLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_info_app_info_localizations_linkages_response import AppInfoAppInfoLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfoAppInfoLocalizationsLinkagesResponse from a JSON string
app_info_app_info_localizations_linkages_response_instance = AppInfoAppInfoLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppInfoAppInfoLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
app_info_app_info_localizations_linkages_response_dict = app_info_app_info_localizations_linkages_response_instance.to_dict()
# create an instance of AppInfoAppInfoLocalizationsLinkagesResponse from a dict
app_info_app_info_localizations_linkages_response_from_dict = AppInfoAppInfoLocalizationsLinkagesResponse.from_dict(app_info_app_info_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


