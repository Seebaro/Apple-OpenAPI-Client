# SubscriptionGroupLocalization


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
from openapi_client.models.subscription_group_localization import SubscriptionGroupLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalization from a JSON string
subscription_group_localization_instance = SubscriptionGroupLocalization.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalization.to_json())

# convert the object into a dict
subscription_group_localization_dict = subscription_group_localization_instance.to_dict()
# create an instance of SubscriptionGroupLocalization from a dict
subscription_group_localization_from_dict = SubscriptionGroupLocalization.from_dict(subscription_group_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


