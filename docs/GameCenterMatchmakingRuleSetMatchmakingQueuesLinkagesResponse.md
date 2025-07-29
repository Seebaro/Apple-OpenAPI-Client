# GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingRuleSetRelationshipsMatchmakingQueuesDataInner]**](GameCenterMatchmakingRuleSetRelationshipsMatchmakingQueuesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_matchmaking_queues_linkages_response import GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse from a JSON string
game_center_matchmaking_rule_set_matchmaking_queues_linkages_response_instance = GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_matchmaking_queues_linkages_response_dict = game_center_matchmaking_rule_set_matchmaking_queues_linkages_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse from a dict
game_center_matchmaking_rule_set_matchmaking_queues_linkages_response_from_dict = GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse.from_dict(game_center_matchmaking_rule_set_matchmaking_queues_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


