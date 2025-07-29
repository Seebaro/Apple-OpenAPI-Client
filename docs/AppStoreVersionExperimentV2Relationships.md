# AppStoreVersionExperimentV2Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**latest_control_version** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**control_versions** | [**AppStoreVersionExperimentV2RelationshipsControlVersions**](AppStoreVersionExperimentV2RelationshipsControlVersions.md) |  | [optional] 
**app_store_version_experiment_treatments** | [**AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments**](AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_relationships import AppStoreVersionExperimentV2Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2Relationships from a JSON string
app_store_version_experiment_v2_relationships_instance = AppStoreVersionExperimentV2Relationships.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2Relationships.to_json())

# convert the object into a dict
app_store_version_experiment_v2_relationships_dict = app_store_version_experiment_v2_relationships_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2Relationships from a dict
app_store_version_experiment_v2_relationships_from_dict = AppStoreVersionExperimentV2Relationships.from_dict(app_store_version_experiment_v2_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


