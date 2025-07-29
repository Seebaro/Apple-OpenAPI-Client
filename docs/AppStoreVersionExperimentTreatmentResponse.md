# AppStoreVersionExperimentTreatmentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionExperimentTreatment**](AppStoreVersionExperimentTreatment.md) |  | 
**included** | [**List[AppStoreVersionExperimentTreatmentsResponseIncludedInner]**](AppStoreVersionExperimentTreatmentsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_response import AppStoreVersionExperimentTreatmentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentResponse from a JSON string
app_store_version_experiment_treatment_response_instance = AppStoreVersionExperimentTreatmentResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentResponse.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_response_dict = app_store_version_experiment_treatment_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentResponse from a dict
app_store_version_experiment_treatment_response_from_dict = AppStoreVersionExperimentTreatmentResponse.from_dict(app_store_version_experiment_treatment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


