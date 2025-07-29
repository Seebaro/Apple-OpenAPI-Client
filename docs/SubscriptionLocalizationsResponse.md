# SubscriptionLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionLocalization]**](SubscriptionLocalization.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_localizations_response import SubscriptionLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalizationsResponse from a JSON string
subscription_localizations_response_instance = SubscriptionLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalizationsResponse.to_json())

# convert the object into a dict
subscription_localizations_response_dict = subscription_localizations_response_instance.to_dict()
# create an instance of SubscriptionLocalizationsResponse from a dict
subscription_localizations_response_from_dict = SubscriptionLocalizationsResponse.from_dict(subscription_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


