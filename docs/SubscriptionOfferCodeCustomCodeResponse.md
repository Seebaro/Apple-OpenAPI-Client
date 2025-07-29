# SubscriptionOfferCodeCustomCodeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCodeCustomCode**](SubscriptionOfferCodeCustomCode.md) |  | 
**included** | [**List[SubscriptionOfferCode]**](SubscriptionOfferCode.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_custom_code_response import SubscriptionOfferCodeCustomCodeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCustomCodeResponse from a JSON string
subscription_offer_code_custom_code_response_instance = SubscriptionOfferCodeCustomCodeResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCustomCodeResponse.to_json())

# convert the object into a dict
subscription_offer_code_custom_code_response_dict = subscription_offer_code_custom_code_response_instance.to_dict()
# create an instance of SubscriptionOfferCodeCustomCodeResponse from a dict
subscription_offer_code_custom_code_response_from_dict = SubscriptionOfferCodeCustomCodeResponse.from_dict(subscription_offer_code_custom_code_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


