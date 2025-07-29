# AppStoreVersionLocalizationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPreviewSetAttributes**](AppPreviewSetAttributes.md) |  | [optional] 
**relationships** | [**AppPreviewSetRelationships**](AppPreviewSetRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_localizations_response_included_inner import AppStoreVersionLocalizationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionLocalizationsResponseIncludedInner from a JSON string
app_store_version_localizations_response_included_inner_instance = AppStoreVersionLocalizationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionLocalizationsResponseIncludedInner.to_json())

# convert the object into a dict
app_store_version_localizations_response_included_inner_dict = app_store_version_localizations_response_included_inner_instance.to_dict()
# create an instance of AppStoreVersionLocalizationsResponseIncludedInner from a dict
app_store_version_localizations_response_included_inner_from_dict = AppStoreVersionLocalizationsResponseIncludedInner.from_dict(app_store_version_localizations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


