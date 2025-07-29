# AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPreviewSetRelationshipsAppStoreVersionLocalizationData]**](AppPreviewSetRelationshipsAppStoreVersionLocalizationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_app_store_version_localizations_linkages_response import AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse from a JSON string
app_store_version_app_store_version_localizations_linkages_response_instance = AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
app_store_version_app_store_version_localizations_linkages_response_dict = app_store_version_app_store_version_localizations_linkages_response_instance.to_dict()
# create an instance of AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse from a dict
app_store_version_app_store_version_localizations_linkages_response_from_dict = AppStoreVersionAppStoreVersionLocalizationsLinkagesResponse.from_dict(app_store_version_app_store_version_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


