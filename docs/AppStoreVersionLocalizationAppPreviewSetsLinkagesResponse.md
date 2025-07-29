# AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCustomProductPageLocalizationRelationshipsAppPreviewSetsDataInner]**](AppCustomProductPageLocalizationRelationshipsAppPreviewSetsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_localization_app_preview_sets_linkages_response import AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse from a JSON string
app_store_version_localization_app_preview_sets_linkages_response_instance = AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.to_json())

# convert the object into a dict
app_store_version_localization_app_preview_sets_linkages_response_dict = app_store_version_localization_app_preview_sets_linkages_response_instance.to_dict()
# create an instance of AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse from a dict
app_store_version_localization_app_preview_sets_linkages_response_from_dict = AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.from_dict(app_store_version_localization_app_preview_sets_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


