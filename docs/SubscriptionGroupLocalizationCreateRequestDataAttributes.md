# SubscriptionGroupLocalizationCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**custom_app_name** | **str** |  | [optional] 
**locale** | **str** |  | 

## Example

```python
from openapi_client.models.subscription_group_localization_create_request_data_attributes import SubscriptionGroupLocalizationCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationCreateRequestDataAttributes from a JSON string
subscription_group_localization_create_request_data_attributes_instance = SubscriptionGroupLocalizationCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationCreateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_group_localization_create_request_data_attributes_dict = subscription_group_localization_create_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationCreateRequestDataAttributes from a dict
subscription_group_localization_create_request_data_attributes_from_dict = SubscriptionGroupLocalizationCreateRequestDataAttributes.from_dict(subscription_group_localization_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


