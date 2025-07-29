# GameCenterChallengeVersionReleaseCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**GameCenterChallengeVersionReleaseCreateRequestDataRelationships**](GameCenterChallengeVersionReleaseCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_version_release_create_request_data import GameCenterChallengeVersionReleaseCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionReleaseCreateRequestData from a JSON string
game_center_challenge_version_release_create_request_data_instance = GameCenterChallengeVersionReleaseCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionReleaseCreateRequestData.to_json())

# convert the object into a dict
game_center_challenge_version_release_create_request_data_dict = game_center_challenge_version_release_create_request_data_instance.to_dict()
# create an instance of GameCenterChallengeVersionReleaseCreateRequestData from a dict
game_center_challenge_version_release_create_request_data_from_dict = GameCenterChallengeVersionReleaseCreateRequestData.from_dict(game_center_challenge_version_release_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


