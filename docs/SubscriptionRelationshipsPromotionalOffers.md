# SubscriptionRelationshipsPromotionalOffers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionRelationshipsPromotionalOffersDataInner]**](SubscriptionRelationshipsPromotionalOffersDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_promotional_offers import SubscriptionRelationshipsPromotionalOffers

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsPromotionalOffers from a JSON string
subscription_relationships_promotional_offers_instance = SubscriptionRelationshipsPromotionalOffers.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsPromotionalOffers.to_json())

# convert the object into a dict
subscription_relationships_promotional_offers_dict = subscription_relationships_promotional_offers_instance.to_dict()
# create an instance of SubscriptionRelationshipsPromotionalOffers from a dict
subscription_relationships_promotional_offers_from_dict = SubscriptionRelationshipsPromotionalOffers.from_dict(subscription_relationships_promotional_offers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


