# GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **datetime** |  | [optional] 
**end** | **datetime** |  | [optional] 
**values** | [**GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPointsValues**](GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPointsValues.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points import GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints from a JSON string
game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points_instance = GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints.to_json())

# convert the object into a dict
game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points_dict = game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints from a dict
game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points_from_dict = GameCenterMatchmakingQueueSizesV1MetricResponseDataInnerDataPoints.from_dict(game_center_matchmaking_queue_sizes_v1_metric_response_data_inner_data_points_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


