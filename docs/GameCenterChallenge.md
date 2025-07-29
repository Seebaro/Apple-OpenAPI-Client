# GameCenterChallenge


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterChallengeAttributes**](GameCenterChallengeAttributes.md) |  | [optional] 
**relationships** | [**GameCenterChallengeRelationships**](GameCenterChallengeRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge import GameCenterChallenge

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallenge from a JSON string
game_center_challenge_instance = GameCenterChallenge.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallenge.to_json())

# convert the object into a dict
game_center_challenge_dict = game_center_challenge_instance.to_dict()
# create an instance of GameCenterChallenge from a dict
game_center_challenge_from_dict = GameCenterChallenge.from_dict(game_center_challenge_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


