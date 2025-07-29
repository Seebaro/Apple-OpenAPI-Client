# AppStoreVersionExperimentTreatmentAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**app_icon** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**app_icon_name** | **str** |  | [optional] 
**promoted_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatment_attributes import AppStoreVersionExperimentTreatmentAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentAttributes from a JSON string
app_store_version_experiment_treatment_attributes_instance = AppStoreVersionExperimentTreatmentAttributes.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentAttributes.to_json())

# convert the object into a dict
app_store_version_experiment_treatment_attributes_dict = app_store_version_experiment_treatment_attributes_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentAttributes from a dict
app_store_version_experiment_treatment_attributes_from_dict = AppStoreVersionExperimentTreatmentAttributes.from_dict(app_store_version_experiment_treatment_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


