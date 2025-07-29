# GameCenterChallengeImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallengeImage**](GameCenterChallengeImage.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_image_response import GameCenterChallengeImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeImageResponse from a JSON string
game_center_challenge_image_response_instance = GameCenterChallengeImageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeImageResponse.to_json())

# convert the object into a dict
game_center_challenge_image_response_dict = game_center_challenge_image_response_instance.to_dict()
# create an instance of GameCenterChallengeImageResponse from a dict
game_center_challenge_image_response_from_dict = GameCenterChallengeImageResponse.from_dict(game_center_challenge_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


