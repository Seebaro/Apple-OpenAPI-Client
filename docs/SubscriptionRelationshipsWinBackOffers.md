# SubscriptionRelationshipsWinBackOffers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionRelationshipsWinBackOffersDataInner]**](SubscriptionRelationshipsWinBackOffersDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_win_back_offers import SubscriptionRelationshipsWinBackOffers

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsWinBackOffers from a JSON string
subscription_relationships_win_back_offers_instance = SubscriptionRelationshipsWinBackOffers.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsWinBackOffers.to_json())

# convert the object into a dict
subscription_relationships_win_back_offers_dict = subscription_relationships_win_back_offers_instance.to_dict()
# create an instance of SubscriptionRelationshipsWinBackOffers from a dict
subscription_relationships_win_back_offers_from_dict = SubscriptionRelationshipsWinBackOffers.from_dict(subscription_relationships_win_back_offers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


