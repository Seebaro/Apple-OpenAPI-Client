# InAppPurchasePriceInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**InAppPurchasePriceInlineCreateAttributes**](InAppPurchasePriceInlineCreateAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePriceInlineCreateRelationships**](InAppPurchasePriceInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_inline_create import InAppPurchasePriceInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceInlineCreate from a JSON string
in_app_purchase_price_inline_create_instance = InAppPurchasePriceInlineCreate.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceInlineCreate.to_json())

# convert the object into a dict
in_app_purchase_price_inline_create_dict = in_app_purchase_price_inline_create_instance.to_dict()
# create an instance of InAppPurchasePriceInlineCreate from a dict
in_app_purchase_price_inline_create_from_dict = InAppPurchasePriceInlineCreate.from_dict(in_app_purchase_price_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


