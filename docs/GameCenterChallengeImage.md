# GameCenterChallengeImage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementImageAttributes**](GameCenterAchievementImageAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_image import GameCenterChallengeImage

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeImage from a JSON string
game_center_challenge_image_instance = GameCenterChallengeImage.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeImage.to_json())

# convert the object into a dict
game_center_challenge_image_dict = game_center_challenge_image_instance.to_dict()
# create an instance of GameCenterChallengeImage from a dict
game_center_challenge_image_from_dict = GameCenterChallengeImage.from_dict(game_center_challenge_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


