# AppStoreVersionExperimentTreatmentsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentTreatment]**](AppStoreVersionExperimentTreatment.md) |  | 
**included** | [**List[AppStoreVersionExperimentTreatmentsResponseIncludedInner]**](AppStoreVersionExperimentTreatmentsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_treatments_response import AppStoreVersionExperimentTreatmentsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentTreatmentsResponse from a JSON string
app_store_version_experiment_treatments_response_instance = AppStoreVersionExperimentTreatmentsResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentTreatmentsResponse.to_json())

# convert the object into a dict
app_store_version_experiment_treatments_response_dict = app_store_version_experiment_treatments_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentTreatmentsResponse from a dict
app_store_version_experiment_treatments_response_from_dict = AppStoreVersionExperimentTreatmentsResponse.from_dict(app_store_version_experiment_treatments_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


