# GameCenterActivityLeaderboardsLinkagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterActivityRelationshipsLeaderboardsDataInner]**](GameCenterActivityRelationshipsLeaderboardsDataInner.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_leaderboards_linkages_request import GameCenterActivityLeaderboardsLinkagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityLeaderboardsLinkagesRequest from a JSON string
game_center_activity_leaderboards_linkages_request_instance = GameCenterActivityLeaderboardsLinkagesRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityLeaderboardsLinkagesRequest.to_json())

# convert the object into a dict
game_center_activity_leaderboards_linkages_request_dict = game_center_activity_leaderboards_linkages_request_instance.to_dict()
# create an instance of GameCenterActivityLeaderboardsLinkagesRequest from a dict
game_center_activity_leaderboards_linkages_request_from_dict = GameCenterActivityLeaderboardsLinkagesRequest.from_dict(game_center_activity_leaderboards_linkages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


