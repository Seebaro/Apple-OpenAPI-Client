# MarketplaceSearchDetailUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceSearchDetailUpdateRequestData**](MarketplaceSearchDetailUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.marketplace_search_detail_update_request import MarketplaceSearchDetailUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetailUpdateRequest from a JSON string
marketplace_search_detail_update_request_instance = MarketplaceSearchDetailUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetailUpdateRequest.to_json())

# convert the object into a dict
marketplace_search_detail_update_request_dict = marketplace_search_detail_update_request_instance.to_dict()
# create an instance of MarketplaceSearchDetailUpdateRequest from a dict
marketplace_search_detail_update_request_from_dict = MarketplaceSearchDetailUpdateRequest.from_dict(marketplace_search_detail_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


