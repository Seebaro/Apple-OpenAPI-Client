# AppStoreVersionPromotion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_promotion import AppStoreVersionPromotion

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionPromotion from a JSON string
app_store_version_promotion_instance = AppStoreVersionPromotion.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionPromotion.to_json())

# convert the object into a dict
app_store_version_promotion_dict = app_store_version_promotion_instance.to_dict()
# create an instance of AppStoreVersionPromotion from a dict
app_store_version_promotion_from_dict = AppStoreVersionPromotion.from_dict(app_store_version_promotion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


