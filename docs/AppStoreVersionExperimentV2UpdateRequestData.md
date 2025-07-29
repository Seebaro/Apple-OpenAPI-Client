# AppStoreVersionExperimentV2UpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentV2UpdateRequestDataAttributes**](AppStoreVersionExperimentV2UpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_update_request_data import AppStoreVersionExperimentV2UpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2UpdateRequestData from a JSON string
app_store_version_experiment_v2_update_request_data_instance = AppStoreVersionExperimentV2UpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2UpdateRequestData.to_json())

# convert the object into a dict
app_store_version_experiment_v2_update_request_data_dict = app_store_version_experiment_v2_update_request_data_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2UpdateRequestData from a dict
app_store_version_experiment_v2_update_request_data_from_dict = AppStoreVersionExperimentV2UpdateRequestData.from_dict(app_store_version_experiment_v2_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


