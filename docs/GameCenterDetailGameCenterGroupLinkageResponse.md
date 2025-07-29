# GameCenterDetailGameCenterGroupLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAchievementRelationshipsGameCenterGroupData**](GameCenterAchievementRelationshipsGameCenterGroupData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_detail_game_center_group_linkage_response import GameCenterDetailGameCenterGroupLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailGameCenterGroupLinkageResponse from a JSON string
game_center_detail_game_center_group_linkage_response_instance = GameCenterDetailGameCenterGroupLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailGameCenterGroupLinkageResponse.to_json())

# convert the object into a dict
game_center_detail_game_center_group_linkage_response_dict = game_center_detail_game_center_group_linkage_response_instance.to_dict()
# create an instance of GameCenterDetailGameCenterGroupLinkageResponse from a dict
game_center_detail_game_center_group_linkage_response_from_dict = GameCenterDetailGameCenterGroupLinkageResponse.from_dict(game_center_detail_game_center_group_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


