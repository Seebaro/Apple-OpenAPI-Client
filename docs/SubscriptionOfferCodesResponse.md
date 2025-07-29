# SubscriptionOfferCodesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionOfferCode]**](SubscriptionOfferCode.md) |  | 
**included** | [**List[SubscriptionOfferCodesResponseIncludedInner]**](SubscriptionOfferCodesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_codes_response import SubscriptionOfferCodesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodesResponse from a JSON string
subscription_offer_codes_response_instance = SubscriptionOfferCodesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodesResponse.to_json())

# convert the object into a dict
subscription_offer_codes_response_dict = subscription_offer_codes_response_instance.to_dict()
# create an instance of SubscriptionOfferCodesResponse from a dict
subscription_offer_codes_response_from_dict = SubscriptionOfferCodesResponse.from_dict(subscription_offer_codes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


