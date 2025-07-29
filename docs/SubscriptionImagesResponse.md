# SubscriptionImagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionImage]**](SubscriptionImage.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_images_response import SubscriptionImagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImagesResponse from a JSON string
subscription_images_response_instance = SubscriptionImagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImagesResponse.to_json())

# convert the object into a dict
subscription_images_response_dict = subscription_images_response_instance.to_dict()
# create an instance of SubscriptionImagesResponse from a dict
subscription_images_response_from_dict = SubscriptionImagesResponse.from_dict(subscription_images_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


