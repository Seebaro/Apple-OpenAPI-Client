# AppStoreVersionReleaseRequestResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionReleaseRequest**](AppStoreVersionReleaseRequest.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_release_request_response import AppStoreVersionReleaseRequestResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionReleaseRequestResponse from a JSON string
app_store_version_release_request_response_instance = AppStoreVersionReleaseRequestResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionReleaseRequestResponse.to_json())

# convert the object into a dict
app_store_version_release_request_response_dict = app_store_version_release_request_response_instance.to_dict()
# create an instance of AppStoreVersionReleaseRequestResponse from a dict
app_store_version_release_request_response_from_dict = AppStoreVersionReleaseRequestResponse.from_dict(app_store_version_release_request_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


