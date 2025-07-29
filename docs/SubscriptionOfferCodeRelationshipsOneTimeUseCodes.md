# SubscriptionOfferCodeRelationshipsOneTimeUseCodes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionOfferCodeRelationshipsOneTimeUseCodesDataInner]**](SubscriptionOfferCodeRelationshipsOneTimeUseCodesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_relationships_one_time_use_codes import SubscriptionOfferCodeRelationshipsOneTimeUseCodes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeRelationshipsOneTimeUseCodes from a JSON string
subscription_offer_code_relationships_one_time_use_codes_instance = SubscriptionOfferCodeRelationshipsOneTimeUseCodes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeRelationshipsOneTimeUseCodes.to_json())

# convert the object into a dict
subscription_offer_code_relationships_one_time_use_codes_dict = subscription_offer_code_relationships_one_time_use_codes_instance.to_dict()
# create an instance of SubscriptionOfferCodeRelationshipsOneTimeUseCodes from a dict
subscription_offer_code_relationships_one_time_use_codes_from_dict = SubscriptionOfferCodeRelationshipsOneTimeUseCodes.from_dict(subscription_offer_code_relationships_one_time_use_codes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


