# AppStoreVersionReleaseRequestCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**AlternativeDistributionPackageCreateRequestDataRelationships**](AlternativeDistributionPackageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_release_request_create_request_data import AppStoreVersionReleaseRequestCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionReleaseRequestCreateRequestData from a JSON string
app_store_version_release_request_create_request_data_instance = AppStoreVersionReleaseRequestCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionReleaseRequestCreateRequestData.to_json())

# convert the object into a dict
app_store_version_release_request_create_request_data_dict = app_store_version_release_request_create_request_data_instance.to_dict()
# create an instance of AppStoreVersionReleaseRequestCreateRequestData from a dict
app_store_version_release_request_create_request_data_from_dict = AppStoreVersionReleaseRequestCreateRequestData.from_dict(app_store_version_release_request_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


