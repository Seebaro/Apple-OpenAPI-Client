# AppStoreVersionExperimentTreatmentLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentLocalizationAttributes**](AppStoreVersionExperimentTreatmentLocalizationAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentTreatmentLocalizationRelationships**](AppStoreVersionExperimentTreatmentLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_localization import AppStoreVersionExperimentTreatmentLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentLocalization from a JSON string
app_store_version_experiment_treatment_localization_instance = AppStoreVersionExperimentTreatmentLocalization.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentLocalization.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_localization_dict = app_store_version_experiment_treatment_localization_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentLocalization from a dict
app_store_version_experiment_treatment_localization_from_dict = AppStoreVersionExperimentTreatmentLocalization.from_dict(app_store_version_experiment_treatment_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


