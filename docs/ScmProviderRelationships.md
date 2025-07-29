# ScmProviderRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**repositories** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_provider_relationships import ScmProviderRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProviderRelationships from a JSON string
scm_provider_relationships_instance = ScmProviderRelationships.from_json(json)
# print the JSON string representation of the object
print(ScmProviderRelationships.to_json())

# convert the object into a dict
scm_provider_relationships_dict = scm_provider_relationships_instance.to_dict()
# create an instance of ScmProviderRelationships from a dict
scm_provider_relationships_from_dict = ScmProviderRelationships.from_dict(scm_provider_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


