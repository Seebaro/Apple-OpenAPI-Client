# GameCenterAchievementImageAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**image_asset** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_image_attributes import GameCenterAchievementImageAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementImageAttributes from a JSON string
game_center_achievement_image_attributes_instance = GameCenterAchievementImageAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementImageAttributes.to_json())

# convert the object into a dict
game_center_achievement_image_attributes_dict = game_center_achievement_image_attributes_instance.to_dict()
# create an instance of GameCenterAchievementImageAttributes from a dict
game_center_achievement_image_attributes_from_dict = GameCenterAchievementImageAttributes.from_dict(game_center_achievement_image_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


