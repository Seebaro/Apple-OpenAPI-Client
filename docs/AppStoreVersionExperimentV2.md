# AppStoreVersionExperimentV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentV2Attributes**](AppStoreVersionExperimentV2Attributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentV2Relationships**](AppStoreVersionExperimentV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2 import AppStoreVersionExperimentV2

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2 from a JSON string
app_store_version_experiment_v2_instance = AppStoreVersionExperimentV2.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2.to_json())

# convert the object into a dict
app_store_version_experiment_v2_dict = app_store_version_experiment_v2_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2 from a dict
app_store_version_experiment_v2_from_dict = AppStoreVersionExperimentV2.from_dict(app_store_version_experiment_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


