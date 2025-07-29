# AppStoreVersionExperimentTreatmentLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionExperimentTreatmentLocalization**](AppStoreVersionExperimentTreatmentLocalization.md) |  | 
**included** | [**List[AppStoreVersionExperimentTreatmentLocalizationsResponseIncludedInner]**](AppStoreVersionExperimentTreatmentLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_localization_response import AppStoreVersionExperimentTreatmentLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentLocalizationResponse from a JSON string
app_store_version_experiment_treatment_localization_response_instance = AppStoreVersionExperimentTreatmentLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentLocalizationResponse.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_localization_response_dict = app_store_version_experiment_treatment_localization_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentLocalizationResponse from a dict
app_store_version_experiment_treatment_localization_response_from_dict = AppStoreVersionExperimentTreatmentLocalizationResponse.from_dict(app_store_version_experiment_treatment_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


