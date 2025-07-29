# AppStoreVersionExperimentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionExperiment**](AppStoreVersionExperiment.md) |  | 
**included** | [**List[AppStoreVersionExperimentsResponseIncludedInner]**](AppStoreVersionExperimentsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_experiment_response import AppStoreVersionExperimentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentResponse from a JSON string
app_store_version_experiment_response_instance = AppStoreVersionExperimentResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentResponse.to_json())

# convert the object into a dict
app_store_version_experiment_response_dict = app_store_version_experiment_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentResponse from a dict
app_store_version_experiment_response_from_dict = AppStoreVersionExperimentResponse.from_dict(app_store_version_experiment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


