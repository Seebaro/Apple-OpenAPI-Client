# AppStoreVersionReleaseRequestCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionReleaseRequestCreateRequestData**](AppStoreVersionReleaseRequestCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_release_request_create_request import AppStoreVersionReleaseRequestCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionReleaseRequestCreateRequest from a JSON string
app_store_version_release_request_create_request_instance = AppStoreVersionReleaseRequestCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionReleaseRequestCreateRequest.to_json())

# convert the object into a dict
app_store_version_release_request_create_request_dict = app_store_version_release_request_create_request_instance.to_dict()
# create an instance of AppStoreVersionReleaseRequestCreateRequest from a dict
app_store_version_release_request_create_request_from_dict = AppStoreVersionReleaseRequestCreateRequest.from_dict(app_store_version_release_request_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


