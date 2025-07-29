# SubscriptionCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**product_id** | **str** |  | 
**family_sharable** | **bool** |  | [optional] 
**subscription_period** | **str** |  | [optional] 
**review_note** | **str** |  | [optional] 
**group_level** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_create_request_data_attributes import SubscriptionCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionCreateRequestDataAttributes from a JSON string
subscription_create_request_data_attributes_instance = SubscriptionCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionCreateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_create_request_data_attributes_dict = subscription_create_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionCreateRequestDataAttributes from a dict
subscription_create_request_data_attributes_from_dict = SubscriptionCreateRequestDataAttributes.from_dict(subscription_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


