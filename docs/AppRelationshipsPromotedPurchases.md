# AppRelationshipsPromotedPurchases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppRelationshipsPromotedPurchasesDataInner]**](AppRelationshipsPromotedPurchasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_promoted_purchases import AppRelationshipsPromotedPurchases

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsPromotedPurchases from a JSON string
app_relationships_promoted_purchases_instance = AppRelationshipsPromotedPurchases.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsPromotedPurchases.to_json())

# convert the object into a dict
app_relationships_promoted_purchases_dict = app_relationships_promoted_purchases_instance.to_dict()
# create an instance of AppRelationshipsPromotedPurchases from a dict
app_relationships_promoted_purchases_from_dict = AppRelationshipsPromotedPurchases.from_dict(app_relationships_promoted_purchases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


