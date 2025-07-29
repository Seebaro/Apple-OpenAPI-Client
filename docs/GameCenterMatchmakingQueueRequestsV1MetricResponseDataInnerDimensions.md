# GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**result** | [**GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDimensionsResult**](GameCenterMatchmakingAppRequestsV1MetricResponseDataInnerDimensionsResult.md) |  | [optional] 
**game_center_detail** | [**AppsBetaTesterUsagesV1MetricResponseDataInnerDimensionsBetaTesters**](AppsBetaTesterUsagesV1MetricResponseDataInnerDimensionsBetaTesters.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions import GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions from a JSON string
game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions_instance = GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions.to_json())

# convert the object into a dict
game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions_dict = game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions from a dict
game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions_from_dict = GameCenterMatchmakingQueueRequestsV1MetricResponseDataInnerDimensions.from_dict(game_center_matchmaking_queue_requests_v1_metric_response_data_inner_dimensions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


