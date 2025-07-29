# SubscriptionImageUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_image_update_request_data import SubscriptionImageUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImageUpdateRequestData from a JSON string
subscription_image_update_request_data_instance = SubscriptionImageUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImageUpdateRequestData.to_json())

# convert the object into a dict
subscription_image_update_request_data_dict = subscription_image_update_request_data_instance.to_dict()
# create an instance of SubscriptionImageUpdateRequestData from a dict
subscription_image_update_request_data_from_dict = SubscriptionImageUpdateRequestData.from_dict(subscription_image_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


