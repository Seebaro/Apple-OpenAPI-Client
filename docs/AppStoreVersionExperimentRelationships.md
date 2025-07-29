# AppStoreVersionExperimentRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_store_version** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**app_store_version_experiment_treatments** | [**AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments**](AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_relationships import AppStoreVersionExperimentRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentRelationships from a JSON string
app_store_version_experiment_relationships_instance = AppStoreVersionExperimentRelationships.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentRelationships.to_json())

# convert the object into a dict
app_store_version_experiment_relationships_dict = app_store_version_experiment_relationships_instance.to_dict()
# create an instance of AppStoreVersionExperimentRelationships from a dict
app_store_version_experiment_relationships_from_dict = AppStoreVersionExperimentRelationships.from_dict(app_store_version_experiment_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


