# AppPriceV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPriceV2Attributes**](AppPriceV2Attributes.md) |  | [optional] 
**relationships** | [**AppPriceV2Relationships**](AppPriceV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_v2 import AppPriceV2

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceV2 from a JSON string
app_price_v2_instance = AppPriceV2.from_json(json)
# print the JSON string representation of the object
print(AppPriceV2.to_json())

# convert the object into a dict
app_price_v2_dict = app_price_v2_instance.to_dict()
# create an instance of AppPriceV2 from a dict
app_price_v2_from_dict = AppPriceV2.from_dict(app_price_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


