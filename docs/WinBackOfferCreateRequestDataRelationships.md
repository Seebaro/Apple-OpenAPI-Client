# WinBackOfferCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**prices** | [**WinBackOfferCreateRequestDataRelationshipsPrices**](WinBackOfferCreateRequestDataRelationshipsPrices.md) |  | 

## Example

```python
from openapi_client.models.win_back_offer_create_request_data_relationships import WinBackOfferCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferCreateRequestDataRelationships from a JSON string
win_back_offer_create_request_data_relationships_instance = WinBackOfferCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferCreateRequestDataRelationships.to_json())

# convert the object into a dict
win_back_offer_create_request_data_relationships_dict = win_back_offer_create_request_data_relationships_instance.to_dict()
# create an instance of WinBackOfferCreateRequestDataRelationships from a dict
win_back_offer_create_request_data_relationships_from_dict = WinBackOfferCreateRequestDataRelationships.from_dict(win_back_offer_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


