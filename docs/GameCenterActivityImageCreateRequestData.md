# GameCenterActivityImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterActivityImageCreateRequestDataRelationships**](GameCenterActivityImageCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_image_create_request_data import GameCenterActivityImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityImageCreateRequestData from a JSON string
game_center_activity_image_create_request_data_instance = GameCenterActivityImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityImageCreateRequestData.to_json())

# convert the object into a dict
game_center_activity_image_create_request_data_dict = game_center_activity_image_create_request_data_instance.to_dict()
# create an instance of GameCenterActivityImageCreateRequestData from a dict
game_center_activity_image_create_request_data_from_dict = GameCenterActivityImageCreateRequestData.from_dict(game_center_activity_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


