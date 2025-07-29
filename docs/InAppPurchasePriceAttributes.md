# InAppPurchasePriceAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 
**manual** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_attributes import InAppPurchasePriceAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceAttributes from a JSON string
in_app_purchase_price_attributes_instance = InAppPurchasePriceAttributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceAttributes.to_json())

# convert the object into a dict
in_app_purchase_price_attributes_dict = in_app_purchase_price_attributes_instance.to_dict()
# create an instance of InAppPurchasePriceAttributes from a dict
in_app_purchase_price_attributes_from_dict = InAppPurchasePriceAttributes.from_dict(in_app_purchase_price_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


