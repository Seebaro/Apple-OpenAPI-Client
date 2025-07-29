# InAppPurchasePrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchasePriceAttributes**](InAppPurchasePriceAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePriceRelationships**](InAppPurchasePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price import InAppPurchasePrice

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePrice from a JSON string
in_app_purchase_price_instance = InAppPurchasePrice.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePrice.to_json())

# convert the object into a dict
in_app_purchase_price_dict = in_app_purchase_price_instance.to_dict()
# create an instance of InAppPurchasePrice from a dict
in_app_purchase_price_from_dict = InAppPurchasePrice.from_dict(in_app_purchase_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


