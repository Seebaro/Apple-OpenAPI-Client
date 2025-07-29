# SubscriptionOfferCodeOneTimeUseCodeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCodeOneTimeUseCode**](SubscriptionOfferCodeOneTimeUseCode.md) |  | 
**included** | [**List[SubscriptionOfferCode]**](SubscriptionOfferCode.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_response import SubscriptionOfferCodeOneTimeUseCodeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeResponse from a JSON string
subscription_offer_code_one_time_use_code_response_instance = SubscriptionOfferCodeOneTimeUseCodeResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeResponse.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_response_dict = subscription_offer_code_one_time_use_code_response_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeResponse from a dict
subscription_offer_code_one_time_use_code_response_from_dict = SubscriptionOfferCodeOneTimeUseCodeResponse.from_dict(subscription_offer_code_one_time_use_code_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


