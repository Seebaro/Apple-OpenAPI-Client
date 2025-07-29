# AgeRatingDeclarationWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AgeRatingDeclaration**](AgeRatingDeclaration.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.age_rating_declaration_without_includes_response import AgeRatingDeclarationWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AgeRatingDeclarationWithoutIncludesResponse from a JSON string
age_rating_declaration_without_includes_response_instance = AgeRatingDeclarationWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(AgeRatingDeclarationWithoutIncludesResponse.to_json())

# convert the object into a dict
age_rating_declaration_without_includes_response_dict = age_rating_declaration_without_includes_response_instance.to_dict()
# create an instance of AgeRatingDeclarationWithoutIncludesResponse from a dict
age_rating_declaration_without_includes_response_from_dict = AgeRatingDeclarationWithoutIncludesResponse.from_dict(age_rating_declaration_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


