# GameCenterChallengeVersionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallengeVersionCreateRequestData**](GameCenterChallengeVersionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_version_create_request import GameCenterChallengeVersionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionCreateRequest from a JSON string
game_center_challenge_version_create_request_instance = GameCenterChallengeVersionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionCreateRequest.to_json())

# convert the object into a dict
game_center_challenge_version_create_request_dict = game_center_challenge_version_create_request_instance.to_dict()
# create an instance of GameCenterChallengeVersionCreateRequest from a dict
game_center_challenge_version_create_request_from_dict = GameCenterChallengeVersionCreateRequest.from_dict(game_center_challenge_version_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


