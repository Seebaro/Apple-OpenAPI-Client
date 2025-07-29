# SubscriptionLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationUpdateRequestDataAttributes**](GameCenterActivityLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_localization_update_request_data import SubscriptionLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalizationUpdateRequestData from a JSON string
subscription_localization_update_request_data_instance = SubscriptionLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalizationUpdateRequestData.to_json())

# convert the object into a dict
subscription_localization_update_request_data_dict = subscription_localization_update_request_data_instance.to_dict()
# create an instance of SubscriptionLocalizationUpdateRequestData from a dict
subscription_localization_update_request_data_from_dict = SubscriptionLocalizationUpdateRequestData.from_dict(subscription_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


