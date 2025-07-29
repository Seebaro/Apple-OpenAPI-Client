# AppPreviewSetsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPreviewAttributes**](AppPreviewAttributes.md) |  | [optional] 
**relationships** | [**AppPreviewRelationships**](AppPreviewRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_preview_sets_response_included_inner import AppPreviewSetsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppPreviewSetsResponseIncludedInner from a JSON string
app_preview_sets_response_included_inner_instance = AppPreviewSetsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppPreviewSetsResponseIncludedInner.to_json())

# convert the object into a dict
app_preview_sets_response_included_inner_dict = app_preview_sets_response_included_inner_instance.to_dict()
# create an instance of AppPreviewSetsResponseIncludedInner from a dict
app_preview_sets_response_included_inner_from_dict = AppPreviewSetsResponseIncludedInner.from_dict(app_preview_sets_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


