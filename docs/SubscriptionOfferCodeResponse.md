# SubscriptionOfferCodeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCode**](SubscriptionOfferCode.md) |  | 
**included** | [**List[SubscriptionOfferCodesResponseIncludedInner]**](SubscriptionOfferCodesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_response import SubscriptionOfferCodeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeResponse from a JSON string
subscription_offer_code_response_instance = SubscriptionOfferCodeResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeResponse.to_json())

# convert the object into a dict
subscription_offer_code_response_dict = subscription_offer_code_response_instance.to_dict()
# create an instance of SubscriptionOfferCodeResponse from a dict
subscription_offer_code_response_from_dict = SubscriptionOfferCodeResponse.from_dict(subscription_offer_code_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


