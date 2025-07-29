# GameCenterChallengeImageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallengeImageCreateRequestData**](GameCenterChallengeImageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_image_create_request import GameCenterChallengeImageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeImageCreateRequest from a JSON string
game_center_challenge_image_create_request_instance = GameCenterChallengeImageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeImageCreateRequest.to_json())

# convert the object into a dict
game_center_challenge_image_create_request_dict = game_center_challenge_image_create_request_instance.to_dict()
# create an instance of GameCenterChallengeImageCreateRequest from a dict
game_center_challenge_image_create_request_from_dict = GameCenterChallengeImageCreateRequest.from_dict(game_center_challenge_image_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


