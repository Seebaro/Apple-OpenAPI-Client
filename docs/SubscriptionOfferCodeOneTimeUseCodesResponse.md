# SubscriptionOfferCodeOneTimeUseCodesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionOfferCodeOneTimeUseCode]**](SubscriptionOfferCodeOneTimeUseCode.md) |  | 
**included** | [**List[SubscriptionOfferCode]**](SubscriptionOfferCode.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_codes_response import SubscriptionOfferCodeOneTimeUseCodesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodesResponse from a JSON string
subscription_offer_code_one_time_use_codes_response_instance = SubscriptionOfferCodeOneTimeUseCodesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodesResponse.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_codes_response_dict = subscription_offer_code_one_time_use_codes_response_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodesResponse from a dict
subscription_offer_code_one_time_use_codes_response_from_dict = SubscriptionOfferCodeOneTimeUseCodesResponse.from_dict(subscription_offer_code_one_time_use_codes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


