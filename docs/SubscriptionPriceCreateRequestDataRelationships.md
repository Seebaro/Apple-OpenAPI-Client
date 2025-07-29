# SubscriptionPriceCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 
**subscription_price_point** | [**SubscriptionPriceCreateRequestDataRelationshipsSubscriptionPricePoint**](SubscriptionPriceCreateRequestDataRelationshipsSubscriptionPricePoint.md) |  | 

## Example

```python
from openapi_client.models.subscription_price_create_request_data_relationships import SubscriptionPriceCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceCreateRequestDataRelationships from a JSON string
subscription_price_create_request_data_relationships_instance = SubscriptionPriceCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceCreateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_price_create_request_data_relationships_dict = subscription_price_create_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionPriceCreateRequestDataRelationships from a dict
subscription_price_create_request_data_relationships_from_dict = SubscriptionPriceCreateRequestDataRelationships.from_dict(subscription_price_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


