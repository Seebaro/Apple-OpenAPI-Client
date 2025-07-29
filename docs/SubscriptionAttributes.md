# SubscriptionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**product_id** | **str** |  | [optional] 
**family_sharable** | **bool** |  | [optional] 
**state** | **str** |  | [optional] 
**subscription_period** | **str** |  | [optional] 
**review_note** | **str** |  | [optional] 
**group_level** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_attributes import SubscriptionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAttributes from a JSON string
subscription_attributes_instance = SubscriptionAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAttributes.to_json())

# convert the object into a dict
subscription_attributes_dict = subscription_attributes_instance.to_dict()
# create an instance of SubscriptionAttributes from a dict
subscription_attributes_from_dict = SubscriptionAttributes.from_dict(subscription_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


