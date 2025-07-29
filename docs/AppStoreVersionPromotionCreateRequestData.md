# AppStoreVersionPromotionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**AppStoreVersionPromotionCreateRequestDataRelationships**](AppStoreVersionPromotionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_promotion_create_request_data import AppStoreVersionPromotionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionPromotionCreateRequestData from a JSON string
app_store_version_promotion_create_request_data_instance = AppStoreVersionPromotionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionPromotionCreateRequestData.to_json())

# convert the object into a dict
app_store_version_promotion_create_request_data_dict = app_store_version_promotion_create_request_data_instance.to_dict()
# create an instance of AppStoreVersionPromotionCreateRequestData from a dict
app_store_version_promotion_create_request_data_from_dict = AppStoreVersionPromotionCreateRequestData.from_dict(app_store_version_promotion_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


