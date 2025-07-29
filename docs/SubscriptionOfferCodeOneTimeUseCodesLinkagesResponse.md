# SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionOfferCodeRelationshipsOneTimeUseCodesDataInner]**](SubscriptionOfferCodeRelationshipsOneTimeUseCodesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_codes_linkages_response import SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse from a JSON string
subscription_offer_code_one_time_use_codes_linkages_response_instance = SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_codes_linkages_response_dict = subscription_offer_code_one_time_use_codes_linkages_response_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse from a dict
subscription_offer_code_one_time_use_codes_linkages_response_from_dict = SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.from_dict(subscription_offer_code_one_time_use_codes_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


