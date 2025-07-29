# GameCenterLeaderboardImageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardImageCreateRequestData**](GameCenterLeaderboardImageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_image_create_request import GameCenterLeaderboardImageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardImageCreateRequest from a JSON string
game_center_leaderboard_image_create_request_instance = GameCenterLeaderboardImageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardImageCreateRequest.to_json())

# convert the object into a dict
game_center_leaderboard_image_create_request_dict = game_center_leaderboard_image_create_request_instance.to_dict()
# create an instance of GameCenterLeaderboardImageCreateRequest from a dict
game_center_leaderboard_image_create_request_from_dict = GameCenterLeaderboardImageCreateRequest.from_dict(game_center_leaderboard_image_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


