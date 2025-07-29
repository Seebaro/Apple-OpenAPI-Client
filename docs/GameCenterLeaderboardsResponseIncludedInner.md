# GameCenterLeaderboardsResponseIncludedInner


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
from openapi_client.models.game_center_leaderboards_response_included_inner import GameCenterLeaderboardsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardsResponseIncludedInner from a JSON string
game_center_leaderboards_response_included_inner_instance = GameCenterLeaderboardsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_leaderboards_response_included_inner_dict = game_center_leaderboards_response_included_inner_instance.to_dict()
# create an instance of GameCenterLeaderboardsResponseIncludedInner from a dict
game_center_leaderboards_response_included_inner_from_dict = GameCenterLeaderboardsResponseIncludedInner.from_dict(game_center_leaderboards_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


