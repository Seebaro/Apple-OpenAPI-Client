# SubscriptionOfferCodeOneTimeUseCodeRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**offer_code** | [**SubscriptionOfferCodeCustomCodeRelationshipsOfferCode**](SubscriptionOfferCodeCustomCodeRelationshipsOfferCode.md) |  | [optional] 
**values** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_relationships import SubscriptionOfferCodeOneTimeUseCodeRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeRelationships from a JSON string
subscription_offer_code_one_time_use_code_relationships_instance = SubscriptionOfferCodeOneTimeUseCodeRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeRelationships.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_relationships_dict = subscription_offer_code_one_time_use_code_relationships_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeRelationships from a dict
subscription_offer_code_one_time_use_code_relationships_from_dict = SubscriptionOfferCodeOneTimeUseCodeRelationships.from_dict(subscription_offer_code_one_time_use_code_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


