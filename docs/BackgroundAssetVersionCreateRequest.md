# BackgroundAssetVersionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetVersionCreateRequestData**](BackgroundAssetVersionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.background_asset_version_create_request import BackgroundAssetVersionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetVersionCreateRequest from a JSON string
background_asset_version_create_request_instance = BackgroundAssetVersionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetVersionCreateRequest.to_json())

# convert the object into a dict
background_asset_version_create_request_dict = background_asset_version_create_request_instance.to_dict()
# create an instance of BackgroundAssetVersionCreateRequest from a dict
background_asset_version_create_request_from_dict = BackgroundAssetVersionCreateRequest.from_dict(background_asset_version_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


