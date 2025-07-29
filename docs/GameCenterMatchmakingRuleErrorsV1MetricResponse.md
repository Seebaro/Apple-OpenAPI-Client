# GameCenterMatchmakingRuleErrorsV1MetricResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingRuleErrorsV1MetricResponseDataInner]**](GameCenterMatchmakingRuleErrorsV1MetricResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_errors_v1_metric_response import GameCenterMatchmakingRuleErrorsV1MetricResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleErrorsV1MetricResponse from a JSON string
game_center_matchmaking_rule_errors_v1_metric_response_instance = GameCenterMatchmakingRuleErrorsV1MetricResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleErrorsV1MetricResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rule_errors_v1_metric_response_dict = game_center_matchmaking_rule_errors_v1_metric_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleErrorsV1MetricResponse from a dict
game_center_matchmaking_rule_errors_v1_metric_response_from_dict = GameCenterMatchmakingRuleErrorsV1MetricResponse.from_dict(game_center_matchmaking_rule_errors_v1_metric_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


