# SubscriptionAvailabilityCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**available_territories** | [**EndUserLicenseAgreementCreateRequestDataRelationshipsTerritories**](EndUserLicenseAgreementCreateRequestDataRelationshipsTerritories.md) |  | 

## Example

```python
from openapi_client.models.subscription_availability_create_request_data_relationships import SubscriptionAvailabilityCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailabilityCreateRequestDataRelationships from a JSON string
subscription_availability_create_request_data_relationships_instance = SubscriptionAvailabilityCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailabilityCreateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_availability_create_request_data_relationships_dict = subscription_availability_create_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionAvailabilityCreateRequestDataRelationships from a dict
subscription_availability_create_request_data_relationships_from_dict = SubscriptionAvailabilityCreateRequestDataRelationships.from_dict(subscription_availability_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


