# InAppPurchaseV2RelationshipsContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**InAppPurchaseV2RelationshipsContentData**](InAppPurchaseV2RelationshipsContentData.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_content import InAppPurchaseV2RelationshipsContent

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsContent from a JSON string
in_app_purchase_v2_relationships_content_instance = InAppPurchaseV2RelationshipsContent.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsContent.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_content_dict = in_app_purchase_v2_relationships_content_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsContent from a dict
in_app_purchase_v2_relationships_content_from_dict = InAppPurchaseV2RelationshipsContent.from_dict(in_app_purchase_v2_relationships_content_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


