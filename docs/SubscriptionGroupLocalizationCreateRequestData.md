# SubscriptionGroupLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionGroupLocalizationCreateRequestDataAttributes**](SubscriptionGroupLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionGroupLocalizationCreateRequestDataRelationships**](SubscriptionGroupLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_localization_create_request_data import SubscriptionGroupLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationCreateRequestData from a JSON string
subscription_group_localization_create_request_data_instance = SubscriptionGroupLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationCreateRequestData.to_json())

# convert the object into a dict
subscription_group_localization_create_request_data_dict = subscription_group_localization_create_request_data_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationCreateRequestData from a dict
subscription_group_localization_create_request_data_from_dict = SubscriptionGroupLocalizationCreateRequestData.from_dict(subscription_group_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


