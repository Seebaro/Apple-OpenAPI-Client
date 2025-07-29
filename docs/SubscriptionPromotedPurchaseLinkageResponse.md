# SubscriptionPromotedPurchaseLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsPromotedPurchasesDataInner**](AppRelationshipsPromotedPurchasesDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_promoted_purchase_linkage_response import SubscriptionPromotedPurchaseLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotedPurchaseLinkageResponse from a JSON string
subscription_promoted_purchase_linkage_response_instance = SubscriptionPromotedPurchaseLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotedPurchaseLinkageResponse.to_json())

# convert the object into a dict
subscription_promoted_purchase_linkage_response_dict = subscription_promoted_purchase_linkage_response_instance.to_dict()
# create an instance of SubscriptionPromotedPurchaseLinkageResponse from a dict
subscription_promoted_purchase_linkage_response_from_dict = SubscriptionPromotedPurchaseLinkageResponse.from_dict(subscription_promoted_purchase_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


