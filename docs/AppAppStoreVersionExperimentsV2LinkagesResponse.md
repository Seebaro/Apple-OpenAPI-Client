# AppAppStoreVersionExperimentsV2LinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData]**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperimentData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_store_version_experiments_v2_linkages_response import AppAppStoreVersionExperimentsV2LinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppStoreVersionExperimentsV2LinkagesResponse from a JSON string
app_app_store_version_experiments_v2_linkages_response_instance = AppAppStoreVersionExperimentsV2LinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppStoreVersionExperimentsV2LinkagesResponse.to_json())

# convert the object into a dict
app_app_store_version_experiments_v2_linkages_response_dict = app_app_store_version_experiments_v2_linkages_response_instance.to_dict()
# create an instance of AppAppStoreVersionExperimentsV2LinkagesResponse from a dict
app_app_store_version_experiments_v2_linkages_response_from_dict = AppAppStoreVersionExperimentsV2LinkagesResponse.from_dict(app_app_store_version_experiments_v2_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


