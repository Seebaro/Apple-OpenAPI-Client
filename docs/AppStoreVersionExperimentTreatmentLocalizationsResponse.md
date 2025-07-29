# AppStoreVersionExperimentTreatmentLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentTreatmentLocalization]**](AppStoreVersionExperimentTreatmentLocalization.md) |  | 
**included** | [**List[AppStoreVersionExperimentTreatmentLocalizationsResponseIncludedInner]**](AppStoreVersionExperimentTreatmentLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_localizations_response import AppStoreVersionExperimentTreatmentLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentLocalizationsResponse from a JSON string
app_store_version_experiment_treatment_localizations_response_instance = AppStoreVersionExperimentTreatmentLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentLocalizationsResponse.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_localizations_response_dict = app_store_version_experiment_treatment_localizations_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentLocalizationsResponse from a dict
app_store_version_experiment_treatment_localizations_response_from_dict = AppStoreVersionExperimentTreatmentLocalizationsResponse.from_dict(app_store_version_experiment_treatment_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


