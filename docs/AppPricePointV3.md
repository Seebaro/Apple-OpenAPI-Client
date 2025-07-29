# AppPricePointV3


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPricePointV3Attributes**](AppPricePointV3Attributes.md) |  | [optional] 
**relationships** | [**AppPricePointV3Relationships**](AppPricePointV3Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_point_v3 import AppPricePointV3

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointV3 from a JSON string
app_price_point_v3_instance = AppPricePointV3.from_json(json)
# print the JSON string representation of the object
print(AppPricePointV3.to_json())

# convert the object into a dict
app_price_point_v3_dict = app_price_point_v3_instance.to_dict()
# create an instance of AppPricePointV3 from a dict
app_price_point_v3_from_dict = AppPricePointV3.from_dict(app_price_point_v3_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


