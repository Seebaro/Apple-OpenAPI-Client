# AppStoreVersionExperimentUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionExperimentV2UpdateRequestData**](AppStoreVersionExperimentV2UpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_update_request import AppStoreVersionExperimentUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentUpdateRequest from a JSON string
app_store_version_experiment_update_request_instance = AppStoreVersionExperimentUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentUpdateRequest.to_json())

# convert the object into a dict
app_store_version_experiment_update_request_dict = app_store_version_experiment_update_request_instance.to_dict()
# create an instance of AppStoreVersionExperimentUpdateRequest from a dict
app_store_version_experiment_update_request_from_dict = AppStoreVersionExperimentUpdateRequest.from_dict(app_store_version_experiment_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


