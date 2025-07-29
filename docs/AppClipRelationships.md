# AppClipRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**app_clip_default_experiences** | [**AppClipRelationshipsAppClipDefaultExperiences**](AppClipRelationshipsAppClipDefaultExperiences.md) |  | [optional] 
**app_clip_advanced_experiences** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_relationships import AppClipRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipRelationships from a JSON string
app_clip_relationships_instance = AppClipRelationships.from_json(json)
# print the JSON string representation of the object
print(AppClipRelationships.to_json())

# convert the object into a dict
app_clip_relationships_dict = app_clip_relationships_instance.to_dict()
# create an instance of AppClipRelationships from a dict
app_clip_relationships_from_dict = AppClipRelationships.from_dict(app_clip_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


