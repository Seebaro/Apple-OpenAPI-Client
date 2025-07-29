# AppStoreVersionExperimentV2CreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentV2CreateRequestDataAttributes**](AppStoreVersionExperimentV2CreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_v2_create_request_data import AppStoreVersionExperimentV2CreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentV2CreateRequestData from a JSON string
app_store_version_experiment_v2_create_request_data_instance = AppStoreVersionExperimentV2CreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentV2CreateRequestData.to_json())

# convert the object into a dict
app_store_version_experiment_v2_create_request_data_dict = app_store_version_experiment_v2_create_request_data_instance.to_dict()
# create an instance of AppStoreVersionExperimentV2CreateRequestData from a dict
app_store_version_experiment_v2_create_request_data_from_dict = AppStoreVersionExperimentV2CreateRequestData.from_dict(app_store_version_experiment_v2_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


