# BackgroundAssetCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BackgroundAssetCreateRequestData**](BackgroundAssetCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.background_asset_create_request import BackgroundAssetCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetCreateRequest from a JSON string
background_asset_create_request_instance = BackgroundAssetCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetCreateRequest.to_json())

# convert the object into a dict
background_asset_create_request_dict = background_asset_create_request_instance.to_dict()
# create an instance of BackgroundAssetCreateRequest from a dict
background_asset_create_request_from_dict = BackgroundAssetCreateRequest.from_dict(background_asset_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


