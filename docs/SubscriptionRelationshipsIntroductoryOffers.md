# SubscriptionRelationshipsIntroductoryOffers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionRelationshipsIntroductoryOffersDataInner]**](SubscriptionRelationshipsIntroductoryOffersDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_introductory_offers import SubscriptionRelationshipsIntroductoryOffers

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsIntroductoryOffers from a JSON string
subscription_relationships_introductory_offers_instance = SubscriptionRelationshipsIntroductoryOffers.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsIntroductoryOffers.to_json())

# convert the object into a dict
subscription_relationships_introductory_offers_dict = subscription_relationships_introductory_offers_instance.to_dict()
# create an instance of SubscriptionRelationshipsIntroductoryOffers from a dict
subscription_relationships_introductory_offers_from_dict = SubscriptionRelationshipsIntroductoryOffers.from_dict(subscription_relationships_introductory_offers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


