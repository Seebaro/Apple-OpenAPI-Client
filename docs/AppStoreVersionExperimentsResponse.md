# AppStoreVersionExperimentsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperiment]**](AppStoreVersionExperiment.md) |  | 
**included** | [**List[AppStoreVersionExperimentsResponseIncludedInner]**](AppStoreVersionExperimentsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiments_response import AppStoreVersionExperimentsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentsResponse from a JSON string
app_store_version_experiments_response_instance = AppStoreVersionExperimentsResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentsResponse.to_json())

# convert the object into a dict
app_store_version_experiments_response_dict = app_store_version_experiments_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentsResponse from a dict
app_store_version_experiments_response_from_dict = AppStoreVersionExperimentsResponse.from_dict(app_store_version_experiments_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


