# GameCenterMatchmakingRulesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingRule]**](GameCenterMatchmakingRule.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rules_response import GameCenterMatchmakingRulesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRulesResponse from a JSON string
game_center_matchmaking_rules_response_instance = GameCenterMatchmakingRulesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRulesResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rules_response_dict = game_center_matchmaking_rules_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRulesResponse from a dict
game_center_matchmaking_rules_response_from_dict = GameCenterMatchmakingRulesResponse.from_dict(game_center_matchmaking_rules_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


