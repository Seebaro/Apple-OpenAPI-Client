# AppStoreVersionExperimentTreatmentUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentUpdateRequestDataAttributes**](AppStoreVersionExperimentTreatmentUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_update_request_data import AppStoreVersionExperimentTreatmentUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentUpdateRequestData from a JSON string
app_store_version_experiment_treatment_update_request_data_instance = AppStoreVersionExperimentTreatmentUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentUpdateRequestData.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_update_request_data_dict = app_store_version_experiment_treatment_update_request_data_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentUpdateRequestData from a dict
app_store_version_experiment_treatment_update_request_data_from_dict = AppStoreVersionExperimentTreatmentUpdateRequestData.from_dict(app_store_version_experiment_treatment_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


