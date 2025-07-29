# GameCenterMatchmakingRuleSetsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingQueueAttributes**](GameCenterMatchmakingQueueAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 
**relationships** | [**GameCenterMatchmakingQueueRelationships**](GameCenterMatchmakingQueueRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_sets_response_included_inner import GameCenterMatchmakingRuleSetsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetsResponseIncludedInner from a JSON string
game_center_matchmaking_rule_sets_response_included_inner_instance = GameCenterMatchmakingRuleSetsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_matchmaking_rule_sets_response_included_inner_dict = game_center_matchmaking_rule_sets_response_included_inner_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetsResponseIncludedInner from a dict
game_center_matchmaking_rule_sets_response_included_inner_from_dict = GameCenterMatchmakingRuleSetsResponseIncludedInner.from_dict(game_center_matchmaking_rule_sets_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


