# NominationRelationshipsSupportedTerritories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppPricePointV3RelationshipsTerritoryData]**](AppPricePointV3RelationshipsTerritoryData.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination_relationships_supported_territories import NominationRelationshipsSupportedTerritories

# TODO update the JSON string below
json = "{}"
# create an instance of NominationRelationshipsSupportedTerritories from a JSON string
nomination_relationships_supported_territories_instance = NominationRelationshipsSupportedTerritories.from_json(json)
# print the JSON string representation of the object
print(NominationRelationshipsSupportedTerritories.to_json())

# convert the object into a dict
nomination_relationships_supported_territories_dict = nomination_relationships_supported_territories_instance.to_dict()
# create an instance of NominationRelationshipsSupportedTerritories from a dict
nomination_relationships_supported_territories_from_dict = NominationRelationshipsSupportedTerritories.from_dict(nomination_relationships_supported_territories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


