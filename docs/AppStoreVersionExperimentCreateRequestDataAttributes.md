# AppStoreVersionExperimentCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**traffic_proportion** | **int** |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_create_request_data_attributes import AppStoreVersionExperimentCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentCreateRequestDataAttributes from a JSON string
app_store_version_experiment_create_request_data_attributes_instance = AppStoreVersionExperimentCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentCreateRequestDataAttributes.to_json())

# convert the object into a dict
app_store_version_experiment_create_request_data_attributes_dict = app_store_version_experiment_create_request_data_attributes_instance.to_dict()
# create an instance of AppStoreVersionExperimentCreateRequestDataAttributes from a dict
app_store_version_experiment_create_request_data_attributes_from_dict = AppStoreVersionExperimentCreateRequestDataAttributes.from_dict(app_store_version_experiment_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


