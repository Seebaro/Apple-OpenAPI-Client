# SubscriptionRelationshipsOfferCodes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionOfferCodeCustomCodeRelationshipsOfferCodeData]**](SubscriptionOfferCodeCustomCodeRelationshipsOfferCodeData.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_offer_codes import SubscriptionRelationshipsOfferCodes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsOfferCodes from a JSON string
subscription_relationships_offer_codes_instance = SubscriptionRelationshipsOfferCodes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsOfferCodes.to_json())

# convert the object into a dict
subscription_relationships_offer_codes_dict = subscription_relationships_offer_codes_instance.to_dict()
# create an instance of SubscriptionRelationshipsOfferCodes from a dict
subscription_relationships_offer_codes_from_dict = SubscriptionRelationshipsOfferCodes.from_dict(subscription_relationships_offer_codes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


