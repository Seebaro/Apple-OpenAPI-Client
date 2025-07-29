# GameCenterAchievementUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAchievementUpdateRequestData**](GameCenterAchievementUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_update_request import GameCenterAchievementUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementUpdateRequest from a JSON string
game_center_achievement_update_request_instance = GameCenterAchievementUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementUpdateRequest.to_json())

# convert the object into a dict
game_center_achievement_update_request_dict = game_center_achievement_update_request_instance.to_dict()
# create an instance of GameCenterAchievementUpdateRequest from a dict
game_center_achievement_update_request_from_dict = GameCenterAchievementUpdateRequest.from_dict(game_center_achievement_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


