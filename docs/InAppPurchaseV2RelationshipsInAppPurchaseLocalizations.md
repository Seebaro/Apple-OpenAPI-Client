# InAppPurchaseV2RelationshipsInAppPurchaseLocalizations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[InAppPurchaseV2RelationshipsInAppPurchaseLocalizationsDataInner]**](InAppPurchaseV2RelationshipsInAppPurchaseLocalizationsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_in_app_purchase_localizations import InAppPurchaseV2RelationshipsInAppPurchaseLocalizations

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsInAppPurchaseLocalizations from a JSON string
in_app_purchase_v2_relationships_in_app_purchase_localizations_instance = InAppPurchaseV2RelationshipsInAppPurchaseLocalizations.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsInAppPurchaseLocalizations.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_in_app_purchase_localizations_dict = in_app_purchase_v2_relationships_in_app_purchase_localizations_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsInAppPurchaseLocalizations from a dict
in_app_purchase_v2_relationships_in_app_purchase_localizations_from_dict = InAppPurchaseV2RelationshipsInAppPurchaseLocalizations.from_dict(in_app_purchase_v2_relationships_in_app_purchase_localizations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


