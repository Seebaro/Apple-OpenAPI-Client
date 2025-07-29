# BackgroundAssetCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**BackgroundAssetCreateRequestDataAttributes**](BackgroundAssetCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.background_asset_create_request_data import BackgroundAssetCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundAssetCreateRequestData from a JSON string
background_asset_create_request_data_instance = BackgroundAssetCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(BackgroundAssetCreateRequestData.to_json())

# convert the object into a dict
background_asset_create_request_data_dict = background_asset_create_request_data_instance.to_dict()
# create an instance of BackgroundAssetCreateRequestData from a dict
background_asset_create_request_data_from_dict = BackgroundAssetCreateRequestData.from_dict(background_asset_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


