# SubscriptionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionCreateRequestDataAttributes**](SubscriptionCreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionCreateRequestDataRelationships**](SubscriptionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_create_request_data import SubscriptionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionCreateRequestData from a JSON string
subscription_create_request_data_instance = SubscriptionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionCreateRequestData.to_json())

# convert the object into a dict
subscription_create_request_data_dict = subscription_create_request_data_instance.to_dict()
# create an instance of SubscriptionCreateRequestData from a dict
subscription_create_request_data_from_dict = SubscriptionCreateRequestData.from_dict(subscription_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


