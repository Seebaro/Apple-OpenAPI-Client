# GameCenterLeaderboardReleaseCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**GameCenterLeaderboardReleaseCreateRequestDataRelationships**](GameCenterLeaderboardReleaseCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_release_create_request_data import GameCenterLeaderboardReleaseCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardReleaseCreateRequestData from a JSON string
game_center_leaderboard_release_create_request_data_instance = GameCenterLeaderboardReleaseCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardReleaseCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_release_create_request_data_dict = game_center_leaderboard_release_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardReleaseCreateRequestData from a dict
game_center_leaderboard_release_create_request_data_from_dict = GameCenterLeaderboardReleaseCreateRequestData.from_dict(game_center_leaderboard_release_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


