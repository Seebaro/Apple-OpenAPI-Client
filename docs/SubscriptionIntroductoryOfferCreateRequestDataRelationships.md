# SubscriptionIntroductoryOfferCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 
**subscription_price_point** | [**SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint**](SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_create_request_data_relationships import SubscriptionIntroductoryOfferCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferCreateRequestDataRelationships from a JSON string
subscription_introductory_offer_create_request_data_relationships_instance = SubscriptionIntroductoryOfferCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferCreateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_introductory_offer_create_request_data_relationships_dict = subscription_introductory_offer_create_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferCreateRequestDataRelationships from a dict
subscription_introductory_offer_create_request_data_relationships_from_dict = SubscriptionIntroductoryOfferCreateRequestDataRelationships.from_dict(subscription_introductory_offer_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


