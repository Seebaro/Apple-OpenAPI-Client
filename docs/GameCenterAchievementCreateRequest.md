# GameCenterAchievementCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAchievementCreateRequestData**](GameCenterAchievementCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_create_request import GameCenterAchievementCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementCreateRequest from a JSON string
game_center_achievement_create_request_instance = GameCenterAchievementCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementCreateRequest.to_json())

# convert the object into a dict
game_center_achievement_create_request_dict = game_center_achievement_create_request_instance.to_dict()
# create an instance of GameCenterAchievementCreateRequest from a dict
game_center_achievement_create_request_from_dict = GameCenterAchievementCreateRequest.from_dict(game_center_achievement_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


