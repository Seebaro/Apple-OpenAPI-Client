# GameCenterChallengeImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterChallengeImageCreateRequestDataRelationships**](GameCenterChallengeImageCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_image_create_request_data import GameCenterChallengeImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeImageCreateRequestData from a JSON string
game_center_challenge_image_create_request_data_instance = GameCenterChallengeImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeImageCreateRequestData.to_json())

# convert the object into a dict
game_center_challenge_image_create_request_data_dict = game_center_challenge_image_create_request_data_instance.to_dict()
# create an instance of GameCenterChallengeImageCreateRequestData from a dict
game_center_challenge_image_create_request_data_from_dict = GameCenterChallengeImageCreateRequestData.from_dict(game_center_challenge_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


