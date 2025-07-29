# SubscriptionAvailabilityCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppAvailabilityV2CreateRequestDataAttributes**](AppAvailabilityV2CreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionAvailabilityCreateRequestDataRelationships**](SubscriptionAvailabilityCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_availability_create_request_data import SubscriptionAvailabilityCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailabilityCreateRequestData from a JSON string
subscription_availability_create_request_data_instance = SubscriptionAvailabilityCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailabilityCreateRequestData.to_json())

# convert the object into a dict
subscription_availability_create_request_data_dict = subscription_availability_create_request_data_instance.to_dict()
# create an instance of SubscriptionAvailabilityCreateRequestData from a dict
subscription_availability_create_request_data_from_dict = SubscriptionAvailabilityCreateRequestData.from_dict(subscription_availability_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


