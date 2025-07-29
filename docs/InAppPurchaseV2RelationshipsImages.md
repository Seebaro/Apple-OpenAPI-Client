# InAppPurchaseV2RelationshipsImages


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[InAppPurchaseV2RelationshipsImagesDataInner]**](InAppPurchaseV2RelationshipsImagesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_images import InAppPurchaseV2RelationshipsImages

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsImages from a JSON string
in_app_purchase_v2_relationships_images_instance = InAppPurchaseV2RelationshipsImages.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsImages.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_images_dict = in_app_purchase_v2_relationships_images_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsImages from a dict
in_app_purchase_v2_relationships_images_from_dict = InAppPurchaseV2RelationshipsImages.from_dict(in_app_purchase_v2_relationships_images_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


