# GameCenterMatchmakingRuleSetRulesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingRuleSetRelationshipsRulesDataInner]**](GameCenterMatchmakingRuleSetRelationshipsRulesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_rules_linkages_response import GameCenterMatchmakingRuleSetRulesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetRulesLinkagesResponse from a JSON string
game_center_matchmaking_rule_set_rules_linkages_response_instance = GameCenterMatchmakingRuleSetRulesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetRulesLinkagesResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_rules_linkages_response_dict = game_center_matchmaking_rule_set_rules_linkages_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetRulesLinkagesResponse from a dict
game_center_matchmaking_rule_set_rules_linkages_response_from_dict = GameCenterMatchmakingRuleSetRulesLinkagesResponse.from_dict(game_center_matchmaking_rule_set_rules_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


