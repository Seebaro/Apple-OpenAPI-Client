# AppRelationshipsInAppPurchasesV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppRelationshipsInAppPurchasesDataInner]**](AppRelationshipsInAppPurchasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_in_app_purchases_v2 import AppRelationshipsInAppPurchasesV2

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsInAppPurchasesV2 from a JSON string
app_relationships_in_app_purchases_v2_instance = AppRelationshipsInAppPurchasesV2.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsInAppPurchasesV2.to_json())

# convert the object into a dict
app_relationships_in_app_purchases_v2_dict = app_relationships_in_app_purchases_v2_instance.to_dict()
# create an instance of AppRelationshipsInAppPurchasesV2 from a dict
app_relationships_in_app_purchases_v2_from_dict = AppRelationshipsInAppPurchasesV2.from_dict(app_relationships_in_app_purchases_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


