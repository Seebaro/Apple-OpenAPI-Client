# SubscriptionGroupLocalizationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**custom_app_name** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_localization_attributes import SubscriptionGroupLocalizationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationAttributes from a JSON string
subscription_group_localization_attributes_instance = SubscriptionGroupLocalizationAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationAttributes.to_json())

# convert the object into a dict
subscription_group_localization_attributes_dict = subscription_group_localization_attributes_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationAttributes from a dict
subscription_group_localization_attributes_from_dict = SubscriptionGroupLocalizationAttributes.from_dict(subscription_group_localization_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


