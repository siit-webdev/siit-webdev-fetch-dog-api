# Homework - fetch information from a public API (https://dog.ceo/dog-api/)

## THE API ENDPOINTS
### List of all available dog breeds
URL: https://dog.ceo/api/breeds/list/all
- The response can be parsed to a JSON object has two properties: *message* and *status*
- The *message* property of the response contains the available breeds **as object properties** (not as an array!)

### Retrieve a random image of a specific breed 
https://dog.ceo/api/breed/{breedName}/images/random
- The *{breedName}* parameter is the breed name, *lowercased*
- Ex. *https://dog.ceo/api/breed/african/images/random*
- The response contains an URL of an image of a dog of the specified breed


### Retrieve a random image of a specific breed 
https://dog.ceo/api/breed/{breedName}/{subBreedName}/images/random
- The *{breedName}* parameter is the breed name, **lowercased**
- The *{subBreedName}* parameter is the sub-breed name, **lowercased**
- Ex. https://dog.ceo/api/breed/australian/shepherd/images/random
- The response contains an URL of an image of a dog of the specified breed and subbreed


## THE HOMEWORK REQUIREMENTS
1. Use fetch to diplay a list containing the available breeds list. *(Optional: when a breed contains a sub-breed, display the sub-breeds as a sub-list of the current element)*
2. When a user clicks on an item in the displayed breed list, the browser, using fetch, should display a random image of the specified list *(Optional: if the sub-breeds are displayed, fetch the specfic sub-breed image)*. 