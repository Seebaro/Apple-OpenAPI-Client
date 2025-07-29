# AppPricePointV3Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**equalizations** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_point_v3_relationships import AppPricePointV3Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointV3Relationships from a JSON string
app_price_point_v3_relationships_instance = AppPricePointV3Relationships.from_json(json)
# print the JSON string representation of the object
print(AppPricePointV3Relationships.to_json())

# convert the object into a dict
app_price_point_v3_relationships_dict = app_price_point_v3_relationships_instance.to_dict()
# create an instance of AppPricePointV3Relationships from a dict
app_price_point_v3_relationships_from_dict = AppPricePointV3Relationships.from_dict(app_price_point_v3_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


