# GameCenterChallengesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterChallenge]**](GameCenterChallenge.md) |  | 
**included** | [**List[GameCenterChallengesResponseIncludedInner]**](GameCenterChallengesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenges_response import GameCenterChallengesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengesResponse from a JSON string
game_center_challenges_response_instance = GameCenterChallengesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengesResponse.to_json())

# convert the object into a dict
game_center_challenges_response_dict = game_center_challenges_response_instance.to_dict()
# create an instance of GameCenterChallengesResponse from a dict
game_center_challenges_response_from_dict = GameCenterChallengesResponse.from_dict(game_center_challenges_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


