# AppStoreVersionExperimentV2Attributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**platform** | [**Platform**](Platform.md) |  | [optional] 
**traffic_proportion** | **int** |  | [optional] 
**state** | **str** |  | [optional] 
**review_required** | **bool** |  | [optional] 
**start_date** | **datetime** |  | [optional] 
**end_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_attributes import AppStoreVersionExperimentV2Attributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2Attributes from a JSON string
app_store_version_experiment_v2_attributes_instance = AppStoreVersionExperimentV2Attributes.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2Attributes.to_json())

# convert the object into a dict
app_store_version_experiment_v2_attributes_dict = app_store_version_experiment_v2_attributes_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2Attributes from a dict
app_store_version_experiment_v2_attributes_from_dict = AppStoreVersionExperimentV2Attributes.from_dict(app_store_version_experiment_v2_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


