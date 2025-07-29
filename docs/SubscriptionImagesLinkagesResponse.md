# SubscriptionImagesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsImagesDataInner]**](SubscriptionRelationshipsImagesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_images_linkages_response import SubscriptionImagesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImagesLinkagesResponse from a JSON string
subscription_images_linkages_response_instance = SubscriptionImagesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImagesLinkagesResponse.to_json())

# convert the object into a dict
subscription_images_linkages_response_dict = subscription_images_linkages_response_instance.to_dict()
# create an instance of SubscriptionImagesLinkagesResponse from a dict
subscription_images_linkages_response_from_dict = SubscriptionImagesLinkagesResponse.from_dict(subscription_images_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


