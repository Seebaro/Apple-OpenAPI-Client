# AppStoreVersionExperimentV2CreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**platform** | [**Platform**](Platform.md) |  | 
**traffic_proportion** | **int** |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_create_request_data_attributes import AppStoreVersionExperimentV2CreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2CreateRequestDataAttributes from a JSON string
app_store_version_experiment_v2_create_request_data_attributes_instance = AppStoreVersionExperimentV2CreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2CreateRequestDataAttributes.to_json())

# convert the object into a dict
app_store_version_experiment_v2_create_request_data_attributes_dict = app_store_version_experiment_v2_create_request_data_attributes_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2CreateRequestDataAttributes from a dict
app_store_version_experiment_v2_create_request_data_attributes_from_dict = AppStoreVersionExperimentV2CreateRequestDataAttributes.from_dict(app_store_version_experiment_v2_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


