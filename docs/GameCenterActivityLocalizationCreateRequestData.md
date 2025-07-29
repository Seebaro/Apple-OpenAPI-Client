# GameCenterActivityLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationCreateRequestDataAttributes**](GameCenterActivityLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterActivityLocalizationCreateRequestDataRelationships**](GameCenterActivityLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_localization_create_request_data import GameCenterActivityLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityLocalizationCreateRequestData from a JSON string
game_center_activity_localization_create_request_data_instance = GameCenterActivityLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityLocalizationCreateRequestData.to_json())

# convert the object into a dict
game_center_activity_localization_create_request_data_dict = game_center_activity_localization_create_request_data_instance.to_dict()
# create an instance of GameCenterActivityLocalizationCreateRequestData from a dict
game_center_activity_localization_create_request_data_from_dict = GameCenterActivityLocalizationCreateRequestData.from_dict(game_center_activity_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


