# SubscriptionGroup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterGroupAttributes**](GameCenterGroupAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionGroupRelationships**](SubscriptionGroupRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group import SubscriptionGroup

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroup from a JSON string
subscription_group_instance = SubscriptionGroup.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroup.to_json())

# convert the object into a dict
subscription_group_dict = subscription_group_instance.to_dict()
# create an instance of SubscriptionGroup from a dict
subscription_group_from_dict = SubscriptionGroup.from_dict(subscription_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


