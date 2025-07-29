# AppStoreVersionExperiment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentAttributes**](AppStoreVersionExperimentAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentRelationships**](AppStoreVersionExperimentRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment import AppStoreVersionExperiment

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperiment from a JSON string
app_store_version_experiment_instance = AppStoreVersionExperiment.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperiment.to_json())

# convert the object into a dict
app_store_version_experiment_dict = app_store_version_experiment_instance.to_dict()
# create an instance of AppStoreVersionExperiment from a dict
app_store_version_experiment_from_dict = AppStoreVersionExperiment.from_dict(app_store_version_experiment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


