# GameCenterAppVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionAttributes**](AppStoreVersionAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionRelationships**](AppStoreVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_app_versions_response_included_inner import GameCenterAppVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionsResponseIncludedInner from a JSON string
game_center_app_versions_response_included_inner_instance = GameCenterAppVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_app_versions_response_included_inner_dict = game_center_app_versions_response_included_inner_instance.to_dict()
# create an instance of GameCenterAppVersionsResponseIncludedInner from a dict
game_center_app_versions_response_included_inner_from_dict = GameCenterAppVersionsResponseIncludedInner.from_dict(game_center_app_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


