# SubscriptionUpdateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**introductory_offers** | [**SubscriptionUpdateRequestDataRelationshipsIntroductoryOffers**](SubscriptionUpdateRequestDataRelationshipsIntroductoryOffers.md) |  | [optional] 
**promotional_offers** | [**SubscriptionUpdateRequestDataRelationshipsPromotionalOffers**](SubscriptionUpdateRequestDataRelationshipsPromotionalOffers.md) |  | [optional] 
**prices** | [**SubscriptionUpdateRequestDataRelationshipsPrices**](SubscriptionUpdateRequestDataRelationshipsPrices.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_update_request_data_relationships import SubscriptionUpdateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionUpdateRequestDataRelationships from a JSON string
subscription_update_request_data_relationships_instance = SubscriptionUpdateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionUpdateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_update_request_data_relationships_dict = subscription_update_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionUpdateRequestDataRelationships from a dict
subscription_update_request_data_relationships_from_dict = SubscriptionUpdateRequestDataRelationships.from_dict(subscription_update_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


