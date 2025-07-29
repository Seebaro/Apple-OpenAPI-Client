# PromotedPurchasesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionAttributes**](SubscriptionAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionRelationships**](SubscriptionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchases_response_included_inner import PromotedPurchasesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchasesResponseIncludedInner from a JSON string
promoted_purchases_response_included_inner_instance = PromotedPurchasesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchasesResponseIncludedInner.to_json())

# convert the object into a dict
promoted_purchases_response_included_inner_dict = promoted_purchases_response_included_inner_instance.to_dict()
# create an instance of PromotedPurchasesResponseIncludedInner from a dict
promoted_purchases_response_included_inner_from_dict = PromotedPurchasesResponseIncludedInner.from_dict(promoted_purchases_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


