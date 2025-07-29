# SubscriptionOfferCodeCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**prices** | [**SubscriptionOfferCodeCreateRequestDataRelationshipsPrices**](SubscriptionOfferCodeCreateRequestDataRelationshipsPrices.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_create_request_data_relationships import SubscriptionOfferCodeCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCreateRequestDataRelationships from a JSON string
subscription_offer_code_create_request_data_relationships_instance = SubscriptionOfferCodeCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCreateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_offer_code_create_request_data_relationships_dict = subscription_offer_code_create_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionOfferCodeCreateRequestDataRelationships from a dict
subscription_offer_code_create_request_data_relationships_from_dict = SubscriptionOfferCodeCreateRequestDataRelationships.from_dict(subscription_offer_code_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


