# SubscriptionGroupsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionGroupLocalizationAttributes**](SubscriptionGroupLocalizationAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionGroupLocalizationRelationships**](SubscriptionGroupLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_groups_response_included_inner import SubscriptionGroupsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupsResponseIncludedInner from a JSON string
subscription_groups_response_included_inner_instance = SubscriptionGroupsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupsResponseIncludedInner.to_json())

# convert the object into a dict
subscription_groups_response_included_inner_dict = subscription_groups_response_included_inner_instance.to_dict()
# create an instance of SubscriptionGroupsResponseIncludedInner from a dict
subscription_groups_response_included_inner_from_dict = SubscriptionGroupsResponseIncludedInner.from_dict(subscription_groups_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


