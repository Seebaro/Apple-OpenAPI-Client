# GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** |  | [optional] 
**average_seconds_in_queue** | **float** |  | [optional] 
**p50_seconds_in_queue** | **float** |  | [optional] 
**p95_seconds_in_queue** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values import GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues from a JSON string
game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values_instance = GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues.to_json())

# convert the object into a dict
game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values_dict = game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values_instance.to_dict()
# create an instance of GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues from a dict
game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values_from_dict = GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDataPointsValues.from_dict(game_center_matchmaking_app_requests_v1_metric_response_data_inner_data_points_values_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


