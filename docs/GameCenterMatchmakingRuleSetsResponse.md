# GameCenterMatchmakingRuleSetsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingRuleSet]**](GameCenterMatchmakingRuleSet.md) |  | 
**included** | [**List[GameCenterMatchmakingRuleSetsResponseIncludedInner]**](GameCenterMatchmakingRuleSetsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_sets_response import GameCenterMatchmakingRuleSetsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetsResponse from a JSON string
game_center_matchmaking_rule_sets_response_instance = GameCenterMatchmakingRuleSetsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetsResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rule_sets_response_dict = game_center_matchmaking_rule_sets_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetsResponse from a dict
game_center_matchmaking_rule_sets_response_from_dict = GameCenterMatchmakingRuleSetsResponse.from_dict(game_center_matchmaking_rule_sets_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


