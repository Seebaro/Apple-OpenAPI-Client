# AppStoreVersionExperimentCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentCreateRequestDataAttributes**](AppStoreVersionExperimentCreateRequestDataAttributes.md) |  | 
**relationships** | [**AlternativeDistributionPackageCreateRequestDataRelationships**](AlternativeDistributionPackageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_create_request_data import AppStoreVersionExperimentCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentCreateRequestData from a JSON string
app_store_version_experiment_create_request_data_instance = AppStoreVersionExperimentCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentCreateRequestData.to_json())

# convert the object into a dict
app_store_version_experiment_create_request_data_dict = app_store_version_experiment_create_request_data_instance.to_dict()
# create an instance of AppStoreVersionExperimentCreateRequestData from a dict
app_store_version_experiment_create_request_data_from_dict = AppStoreVersionExperimentCreateRequestData.from_dict(app_store_version_experiment_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


