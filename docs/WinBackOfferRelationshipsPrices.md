# WinBackOfferRelationshipsPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[WinBackOfferRelationshipsPricesDataInner]**](WinBackOfferRelationshipsPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_relationships_prices import WinBackOfferRelationshipsPrices

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferRelationshipsPrices from a JSON string
win_back_offer_relationships_prices_instance = WinBackOfferRelationshipsPrices.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferRelationshipsPrices.to_json())

# convert the object into a dict
win_back_offer_relationships_prices_dict = win_back_offer_relationships_prices_instance.to_dict()
# create an instance of WinBackOfferRelationshipsPrices from a dict
win_back_offer_relationships_prices_from_dict = WinBackOfferRelationshipsPrices.from_dict(win_back_offer_relationships_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


