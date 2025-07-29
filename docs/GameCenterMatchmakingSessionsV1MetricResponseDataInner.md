# GameCenterMatchmakingSessionsV1MetricResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data_points** | [**GameCenterMatchmakingSessionsV1MetricResponseDataInnerDataPoints**](GameCenterMatchmakingSessionsV1MetricResponseDataInnerDataPoints.md) |  | [optional] 
**granularity** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_sessions_v1_metric_response_data_inner import GameCenterMatchmakingSessionsV1MetricResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingSessionsV1MetricResponseDataInner from a JSON string
game_center_matchmaking_sessions_v1_metric_response_data_inner_instance = GameCenterMatchmakingSessionsV1MetricResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingSessionsV1MetricResponseDataInner.to_json())

# convert the object into a dict
game_center_matchmaking_sessions_v1_metric_response_data_inner_dict = game_center_matchmaking_sessions_v1_metric_response_data_inner_instance.to_dict()
# create an instance of GameCenterMatchmakingSessionsV1MetricResponseDataInner from a dict
game_center_matchmaking_sessions_v1_metric_response_data_inner_from_dict = GameCenterMatchmakingSessionsV1MetricResponseDataInner.from_dict(game_center_matchmaking_sessions_v1_metric_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


