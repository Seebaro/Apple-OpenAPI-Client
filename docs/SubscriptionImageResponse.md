# SubscriptionImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionImage**](SubscriptionImage.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_image_response import SubscriptionImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImageResponse from a JSON string
subscription_image_response_instance = SubscriptionImageResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImageResponse.to_json())

# convert the object into a dict
subscription_image_response_dict = subscription_image_response_instance.to_dict()
# create an instance of SubscriptionImageResponse from a dict
subscription_image_response_from_dict = SubscriptionImageResponse.from_dict(subscription_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


