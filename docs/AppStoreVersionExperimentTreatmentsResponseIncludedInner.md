# AppStoreVersionExperimentTreatmentsResponseIncludedInner


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
from openapi_client.models.app_store_version_experiment_treatments_response_included_inner import AppStoreVersionExperimentTreatmentsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentsResponseIncludedInner from a JSON string
app_store_version_experiment_treatments_response_included_inner_instance = AppStoreVersionExperimentTreatmentsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentsResponseIncludedInner.to_json())

# convert the object into a dict
app_store_version_experiment_treatments_response_included_inner_dict = app_store_version_experiment_treatments_response_included_inner_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentsResponseIncludedInner from a dict
app_store_version_experiment_treatments_response_included_inner_from_dict = AppStoreVersionExperimentTreatmentsResponseIncludedInner.from_dict(app_store_version_experiment_treatments_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


