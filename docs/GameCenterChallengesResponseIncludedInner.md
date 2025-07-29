# GameCenterChallengesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardAttributes**](GameCenterLeaderboardAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardRelationships**](GameCenterLeaderboardRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenges_response_included_inner import GameCenterChallengesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengesResponseIncludedInner from a JSON string
game_center_challenges_response_included_inner_instance = GameCenterChallengesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengesResponseIncludedInner.to_json())

# convert the object into a dict
game_center_challenges_response_included_inner_dict = game_center_challenges_response_included_inner_instance.to_dict()
# create an instance of GameCenterChallengesResponseIncludedInner from a dict
game_center_challenges_response_included_inner_from_dict = GameCenterChallengesResponseIncludedInner.from_dict(game_center_challenges_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


