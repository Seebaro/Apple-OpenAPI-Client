# InAppPurchasePricePointRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 
**equalizations** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_point_relationships import InAppPurchasePricePointRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePricePointRelationships from a JSON string
in_app_purchase_price_point_relationships_instance = InAppPurchasePricePointRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePricePointRelationships.to_json())

# convert the object into a dict
in_app_purchase_price_point_relationships_dict = in_app_purchase_price_point_relationships_instance.to_dict()
# create an instance of InAppPurchasePricePointRelationships from a dict
in_app_purchase_price_point_relationships_from_dict = InAppPurchasePricePointRelationships.from_dict(in_app_purchase_price_point_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


