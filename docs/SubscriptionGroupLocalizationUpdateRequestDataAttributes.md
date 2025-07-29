# SubscriptionGroupLocalizationUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**custom_app_name** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_localization_update_request_data_attributes import SubscriptionGroupLocalizationUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationUpdateRequestDataAttributes from a JSON string
subscription_group_localization_update_request_data_attributes_instance = SubscriptionGroupLocalizationUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationUpdateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_group_localization_update_request_data_attributes_dict = subscription_group_localization_update_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationUpdateRequestDataAttributes from a dict
subscription_group_localization_update_request_data_attributes_from_dict = SubscriptionGroupLocalizationUpdateRequestDataAttributes.from_dict(subscription_group_localization_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


