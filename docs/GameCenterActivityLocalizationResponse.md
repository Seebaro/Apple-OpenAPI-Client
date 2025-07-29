# GameCenterActivityLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityLocalization**](GameCenterActivityLocalization.md) |  | 
**included** | [**List[GameCenterActivityLocalizationsResponseIncludedInner]**](GameCenterActivityLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_localization_response import GameCenterActivityLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityLocalizationResponse from a JSON string
game_center_activity_localization_response_instance = GameCenterActivityLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityLocalizationResponse.to_json())

# convert the object into a dict
game_center_activity_localization_response_dict = game_center_activity_localization_response_instance.to_dict()
# create an instance of GameCenterActivityLocalizationResponse from a dict
game_center_activity_localization_response_from_dict = GameCenterActivityLocalizationResponse.from_dict(game_center_activity_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


