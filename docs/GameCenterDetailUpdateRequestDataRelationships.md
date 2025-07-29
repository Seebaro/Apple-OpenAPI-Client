# GameCenterDetailUpdateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**default_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 
**default_group_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_update_request_data_relationships import GameCenterDetailUpdateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailUpdateRequestDataRelationships from a JSON string
game_center_detail_update_request_data_relationships_instance = GameCenterDetailUpdateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailUpdateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_detail_update_request_data_relationships_dict = game_center_detail_update_request_data_relationships_instance.to_dict()
# create an instance of GameCenterDetailUpdateRequestDataRelationships from a dict
game_center_detail_update_request_data_relationships_from_dict = GameCenterDetailUpdateRequestDataRelationships.from_dict(game_center_detail_update_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


