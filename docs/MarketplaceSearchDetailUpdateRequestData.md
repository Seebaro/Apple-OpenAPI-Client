# MarketplaceSearchDetailUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**MarketplaceSearchDetailAttributes**](MarketplaceSearchDetailAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_search_detail_update_request_data import MarketplaceSearchDetailUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetailUpdateRequestData from a JSON string
marketplace_search_detail_update_request_data_instance = MarketplaceSearchDetailUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetailUpdateRequestData.to_json())

# convert the object into a dict
marketplace_search_detail_update_request_data_dict = marketplace_search_detail_update_request_data_instance.to_dict()
# create an instance of MarketplaceSearchDetailUpdateRequestData from a dict
marketplace_search_detail_update_request_data_from_dict = MarketplaceSearchDetailUpdateRequestData.from_dict(marketplace_search_detail_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


