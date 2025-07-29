# AppStoreVersionExperimentTreatmentCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentCreateRequestDataAttributes**](AppStoreVersionExperimentTreatmentCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppStoreVersionExperimentTreatmentCreateRequestDataRelationships**](AppStoreVersionExperimentTreatmentCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_create_request_data import AppStoreVersionExperimentTreatmentCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentCreateRequestData from a JSON string
app_store_version_experiment_treatment_create_request_data_instance = AppStoreVersionExperimentTreatmentCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentCreateRequestData.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_create_request_data_dict = app_store_version_experiment_treatment_create_request_data_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentCreateRequestData from a dict
app_store_version_experiment_treatment_create_request_data_from_dict = AppStoreVersionExperimentTreatmentCreateRequestData.from_dict(app_store_version_experiment_treatment_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


