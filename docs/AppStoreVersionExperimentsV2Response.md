# AppStoreVersionExperimentsV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentV2]**](AppStoreVersionExperimentV2.md) |  | 
**included** | [**List[AppStoreVersionExperimentsV2ResponseIncludedInner]**](AppStoreVersionExperimentsV2ResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiments_v2_response import AppStoreVersionExperimentsV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentsV2Response from a JSON string
app_store_version_experiments_v2_response_instance = AppStoreVersionExperimentsV2Response.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentsV2Response.to_json())

# convert the object into a dict
app_store_version_experiments_v2_response_dict = app_store_version_experiments_v2_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentsV2Response from a dict
app_store_version_experiments_v2_response_from_dict = AppStoreVersionExperimentsV2Response.from_dict(app_store_version_experiments_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


