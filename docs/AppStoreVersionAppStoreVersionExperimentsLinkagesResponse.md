# AppStoreVersionAppStoreVersionExperimentsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData]**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_app_store_version_experiments_linkages_response import AppStoreVersionAppStoreVersionExperimentsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionAppStoreVersionExperimentsLinkagesResponse from a JSON string
app_store_version_app_store_version_experiments_linkages_response_instance = AppStoreVersionAppStoreVersionExperimentsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionAppStoreVersionExperimentsLinkagesResponse.to_json())

# convert the object into a dict
app_store_version_app_store_version_experiments_linkages_response_dict = app_store_version_app_store_version_experiments_linkages_response_instance.to_dict()
# create an instance of AppStoreVersionAppStoreVersionExperimentsLinkagesResponse from a dict
app_store_version_app_store_version_experiments_linkages_response_from_dict = AppStoreVersionAppStoreVersionExperimentsLinkagesResponse.from_dict(app_store_version_app_store_version_experiments_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


