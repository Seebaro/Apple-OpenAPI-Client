# AppClip


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAttributes**](AppClipAttributes.md) |  | [optional] 
**relationships** | [**AppClipRelationships**](AppClipRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip import AppClip

# TODO update the JSON string below
json = "{}"
# create an instance of AppClip from a JSON string
app_clip_instance = AppClip.from_json(json)
# print the JSON string representation of the object
print(AppClip.to_json())

# convert the object into a dict
app_clip_dict = app_clip_instance.to_dict()
# create an instance of AppClip from a dict
app_clip_from_dict = AppClip.from_dict(app_clip_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


