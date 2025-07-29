# SubscriptionImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_image_create_request_data import SubscriptionImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImageCreateRequestData from a JSON string
subscription_image_create_request_data_instance = SubscriptionImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImageCreateRequestData.to_json())

# convert the object into a dict
subscription_image_create_request_data_dict = subscription_image_create_request_data_instance.to_dict()
# create an instance of SubscriptionImageCreateRequestData from a dict
subscription_image_create_request_data_from_dict = SubscriptionImageCreateRequestData.from_dict(subscription_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


