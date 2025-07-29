# GameCenterChallengeLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallengeLocalization**](GameCenterChallengeLocalization.md) |  | 
**included** | [**List[GameCenterChallengeLocalizationsResponseIncludedInner]**](GameCenterChallengeLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_localization_response import GameCenterChallengeLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeLocalizationResponse from a JSON string
game_center_challenge_localization_response_instance = GameCenterChallengeLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeLocalizationResponse.to_json())

# convert the object into a dict
game_center_challenge_localization_response_dict = game_center_challenge_localization_response_instance.to_dict()
# create an instance of GameCenterChallengeLocalizationResponse from a dict
game_center_challenge_localization_response_from_dict = GameCenterChallengeLocalizationResponse.from_dict(game_center_challenge_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


