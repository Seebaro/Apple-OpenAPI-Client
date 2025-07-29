# SubscriptionUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**family_sharable** | **bool** |  | [optional] 
**subscription_period** | **str** |  | [optional] 
**review_note** | **str** |  | [optional] 
**group_level** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_update_request_data_attributes import SubscriptionUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionUpdateRequestDataAttributes from a JSON string
subscription_update_request_data_attributes_instance = SubscriptionUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionUpdateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_update_request_data_attributes_dict = subscription_update_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionUpdateRequestDataAttributes from a dict
subscription_update_request_data_attributes_from_dict = SubscriptionUpdateRequestDataAttributes.from_dict(subscription_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


