# AppStoreVersionPromotionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionPromotionCreateRequestData**](AppStoreVersionPromotionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_promotion_create_request import AppStoreVersionPromotionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionPromotionCreateRequest from a JSON string
app_store_version_promotion_create_request_instance = AppStoreVersionPromotionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionPromotionCreateRequest.to_json())

# convert the object into a dict
app_store_version_promotion_create_request_dict = app_store_version_promotion_create_request_instance.to_dict()
# create an instance of AppStoreVersionPromotionCreateRequest from a dict
app_store_version_promotion_create_request_from_dict = AppStoreVersionPromotionCreateRequest.from_dict(app_store_version_promotion_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


