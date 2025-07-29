# GameCenterChallengeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallenge**](GameCenterChallenge.md) |  | 
**included** | [**List[GameCenterChallengesResponseIncludedInner]**](GameCenterChallengesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_response import GameCenterChallengeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeResponse from a JSON string
game_center_challenge_response_instance = GameCenterChallengeResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeResponse.to_json())

# convert the object into a dict
game_center_challenge_response_dict = game_center_challenge_response_instance.to_dict()
# create an instance of GameCenterChallengeResponse from a dict
game_center_challenge_response_from_dict = GameCenterChallengeResponse.from_dict(game_center_challenge_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


