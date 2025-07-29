# MarketplaceSearchDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceSearchDetail**](MarketplaceSearchDetail.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.marketplace_search_detail_response import MarketplaceSearchDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSearchDetailResponse from a JSON string
marketplace_search_detail_response_instance = MarketplaceSearchDetailResponse.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSearchDetailResponse.to_json())

# convert the object into a dict
marketplace_search_detail_response_dict = marketplace_search_detail_response_instance.to_dict()
# create an instance of MarketplaceSearchDetailResponse from a dict
marketplace_search_detail_response_from_dict = MarketplaceSearchDetailResponse.from_dict(marketplace_search_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


