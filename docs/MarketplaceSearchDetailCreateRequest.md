# MarketplaceSearchDetailCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceSearchDetailCreateRequestData**](MarketplaceSearchDetailCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.marketplace_search_detail_create_request import MarketplaceSearchDetailCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetailCreateRequest from a JSON string
marketplace_search_detail_create_request_instance = MarketplaceSearchDetailCreateRequest.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetailCreateRequest.to_json())

# convert the object into a dict
marketplace_search_detail_create_request_dict = marketplace_search_detail_create_request_instance.to_dict()
# create an instance of MarketplaceSearchDetailCreateRequest from a dict
marketplace_search_detail_create_request_from_dict = MarketplaceSearchDetailCreateRequest.from_dict(marketplace_search_detail_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


