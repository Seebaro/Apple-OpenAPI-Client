# SubscriptionGroupLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionGroupLocalizationUpdateRequestDataAttributes**](SubscriptionGroupLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_localization_update_request_data import SubscriptionGroupLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationUpdateRequestData from a JSON string
subscription_group_localization_update_request_data_instance = SubscriptionGroupLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationUpdateRequestData.to_json())

# convert the object into a dict
subscription_group_localization_update_request_data_dict = subscription_group_localization_update_request_data_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationUpdateRequestData from a dict
subscription_group_localization_update_request_data_from_dict = SubscriptionGroupLocalizationUpdateRequestData.from_dict(subscription_group_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


