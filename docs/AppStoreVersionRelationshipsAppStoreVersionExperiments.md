# AppStoreVersionRelationshipsAppStoreVersionExperiments


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData]**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_relationships_app_store_version_experiments import AppStoreVersionRelationshipsAppStoreVersionExperiments

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionRelationshipsAppStoreVersionExperiments from a JSON string
app_store_version_relationships_app_store_version_experiments_instance = AppStoreVersionRelationshipsAppStoreVersionExperiments.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionRelationshipsAppStoreVersionExperiments.to_json())

# convert the object into a dict
app_store_version_relationships_app_store_version_experiments_dict = app_store_version_relationships_app_store_version_experiments_instance.to_dict()
# create an instance of AppStoreVersionRelationshipsAppStoreVersionExperiments from a dict
app_store_version_relationships_app_store_version_experiments_from_dict = AppStoreVersionRelationshipsAppStoreVersionExperiments.from_dict(app_store_version_relationships_app_store_version_experiments_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


