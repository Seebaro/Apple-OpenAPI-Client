# AppStoreVersionPromotionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionPromotion**](AppStoreVersionPromotion.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_promotion_response import AppStoreVersionPromotionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionPromotionResponse from a JSON string
app_store_version_promotion_response_instance = AppStoreVersionPromotionResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionPromotionResponse.to_json())

# convert the object into a dict
app_store_version_promotion_response_dict = app_store_version_promotion_response_instance.to_dict()
# create an instance of AppStoreVersionPromotionResponse from a dict
app_store_version_promotion_response_from_dict = AppStoreVersionPromotionResponse.from_dict(app_store_version_promotion_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


