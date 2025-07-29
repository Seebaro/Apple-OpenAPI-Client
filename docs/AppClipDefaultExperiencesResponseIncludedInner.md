# AppClipDefaultExperiencesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAppStoreReviewDetailAttributes**](AppClipAppStoreReviewDetailAttributes.md) |  | [optional] 
**relationships** | [**AppClipAppStoreReviewDetailRelationships**](AppClipAppStoreReviewDetailRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experiences_response_included_inner import AppClipDefaultExperiencesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperiencesResponseIncludedInner from a JSON string
app_clip_default_experiences_response_included_inner_instance = AppClipDefaultExperiencesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperiencesResponseIncludedInner.to_json())

# convert the object into a dict
app_clip_default_experiences_response_included_inner_dict = app_clip_default_experiences_response_included_inner_instance.to_dict()
# create an instance of AppClipDefaultExperiencesResponseIncludedInner from a dict
app_clip_default_experiences_response_included_inner_from_dict = AppClipDefaultExperiencesResponseIncludedInner.from_dict(app_clip_default_experiences_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


