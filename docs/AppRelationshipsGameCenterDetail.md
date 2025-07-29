# AppRelationshipsGameCenterDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**AppRelationshipsGameCenterDetailData**](AppRelationshipsGameCenterDetailData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_game_center_detail import AppRelationshipsGameCenterDetail

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsGameCenterDetail from a JSON string
app_relationships_game_center_detail_instance = AppRelationshipsGameCenterDetail.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsGameCenterDetail.to_json())

# convert the object into a dict
app_relationships_game_center_detail_dict = app_relationships_game_center_detail_instance.to_dict()
# create an instance of AppRelationshipsGameCenterDetail from a dict
app_relationships_game_center_detail_from_dict = AppRelationshipsGameCenterDetail.from_dict(app_relationships_game_center_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


