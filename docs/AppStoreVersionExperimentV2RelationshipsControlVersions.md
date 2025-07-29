# AppStoreVersionExperimentV2RelationshipsControlVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData]**](AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_relationships_control_versions import AppStoreVersionExperimentV2RelationshipsControlVersions

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2RelationshipsControlVersions from a JSON string
app_store_version_experiment_v2_relationships_control_versions_instance = AppStoreVersionExperimentV2RelationshipsControlVersions.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2RelationshipsControlVersions.to_json())

# convert the object into a dict
app_store_version_experiment_v2_relationships_control_versions_dict = app_store_version_experiment_v2_relationships_control_versions_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2RelationshipsControlVersions from a dict
app_store_version_experiment_v2_relationships_control_versions_from_dict = AppStoreVersionExperimentV2RelationshipsControlVersions.from_dict(app_store_version_experiment_v2_relationships_control_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


