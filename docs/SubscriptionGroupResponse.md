# SubscriptionGroupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroup**](SubscriptionGroup.md) |  | 
**included** | [**List[SubscriptionGroupsResponseIncludedInner]**](SubscriptionGroupsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_response import SubscriptionGroupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupResponse from a JSON string
subscription_group_response_instance = SubscriptionGroupResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupResponse.to_json())

# convert the object into a dict
subscription_group_response_dict = subscription_group_response_instance.to_dict()
# create an instance of SubscriptionGroupResponse from a dict
subscription_group_response_from_dict = SubscriptionGroupResponse.from_dict(subscription_group_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


