# AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppStoreVersionExperimentTreatmentLocalizationRelationshipsAppStoreVersionExperimentTreatmentData]**](AppStoreVersionExperimentTreatmentLocalizationRelationshipsAppStoreVersionExperimentTreatmentData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments import AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments from a JSON string
app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments_instance = AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments.to_json())

# convert the object into a dict
app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments_dict = app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments from a dict
app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments_from_dict = AppStoreVersionExperimentV2RelationshipsAppStoreVersionExperimentTreatments.from_dict(app_store_version_experiment_v2_relationships_app_store_version_experiment_treatments_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


