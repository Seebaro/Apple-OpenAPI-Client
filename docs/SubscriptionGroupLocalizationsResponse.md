# SubscriptionGroupLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionGroupLocalization]**](SubscriptionGroupLocalization.md) |  | 
**included** | [**List[SubscriptionGroup]**](SubscriptionGroup.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_localizations_response import SubscriptionGroupLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationsResponse from a JSON string
subscription_group_localizations_response_instance = SubscriptionGroupLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationsResponse.to_json())

# convert the object into a dict
subscription_group_localizations_response_dict = subscription_group_localizations_response_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationsResponse from a dict
subscription_group_localizations_response_from_dict = SubscriptionGroupLocalizationsResponse.from_dict(subscription_group_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


