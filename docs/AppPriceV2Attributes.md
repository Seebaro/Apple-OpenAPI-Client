# AppPriceV2Attributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**manual** | **bool** |  | [optional] 
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 

## Example

```python
from openapi_client.models.app_price_v2_attributes import AppPriceV2Attributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceV2Attributes from a JSON string
app_price_v2_attributes_instance = AppPriceV2Attributes.from_json(json)
# print the JSON string representation of the object
print(AppPriceV2Attributes.to_json())

# convert the object into a dict
app_price_v2_attributes_dict = app_price_v2_attributes_instance.to_dict()
# create an instance of AppPriceV2Attributes from a dict
app_price_v2_attributes_from_dict = AppPriceV2Attributes.from_dict(app_price_v2_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


