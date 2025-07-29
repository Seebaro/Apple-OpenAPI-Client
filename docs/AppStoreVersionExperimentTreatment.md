# AppStoreVersionExperimentTreatment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentAttributes**](AppStoreVersionExperimentTreatmentAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentTreatmentRelationships**](AppStoreVersionExperimentTreatmentRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment import AppStoreVersionExperimentTreatment

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatment from a JSON string
app_store_version_experiment_treatment_instance = AppStoreVersionExperimentTreatment.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatment.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_dict = app_store_version_experiment_treatment_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatment from a dict
app_store_version_experiment_treatment_from_dict = AppStoreVersionExperimentTreatment.from_dict(app_store_version_experiment_treatment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


