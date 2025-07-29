# AppPriceV2Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_price_point** | [**AppPriceV2RelationshipsAppPricePoint**](AppPriceV2RelationshipsAppPricePoint.md) |  | [optional] 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_v2_relationships import AppPriceV2Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceV2Relationships from a JSON string
app_price_v2_relationships_instance = AppPriceV2Relationships.from_json(json)
# print the JSON string representation of the object
print(AppPriceV2Relationships.to_json())

# convert the object into a dict
app_price_v2_relationships_dict = app_price_v2_relationships_instance.to_dict()
# create an instance of AppPriceV2Relationships from a dict
app_price_v2_relationships_from_dict = AppPriceV2Relationships.from_dict(app_price_v2_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


