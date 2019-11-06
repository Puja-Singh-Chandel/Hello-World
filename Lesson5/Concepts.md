# Exploring Advanced UI Interaction
In this practice session, I have learned the concept of different UI Interactions and UiPath's Screen Scarping Wizard and Data Scraping
Wizard. 

## Getting Started
Ui Interactions can be of two types: 
1. Input Interactions: Clicks,Text Typing,Keyboard shortcuts,Right clicks,Mouse hover,etc.
2. Output Interactions: Getting text,Find elemements and images,etc.

## Input Methods

| Input Method        | Compatibility           | Background  | Speed | Hot Key | Empty Field |
| ------------- |:-------------:| -----:| -----:| -----:| -----:|
| Default     | 100%| No | 50% | Yes | No |
| Window Messages      | 80%     | Yes | 50% | Yes | No |
| Simulated Type/click | 95%      | Yes | 100% | No | Yes |

* We should selet the right input method that suits our needs.
* The recommended input method is Simulate because it’s the fastest.
* The recommended output method is FullText because it’s fast and accurate.
* OCR should be only used as a last resort.

## Output Methods

For Simple data extraction we use methods like getText but when there are bigger 
blocks of text, information is behind complex UI or we need exact word position on screen.

| Output Method        | Speed           | Accuracy  | Background | Text Position | Hidden text | Citrix |
| ------------- |:-------------:| -----:| -----:| -----:| -----:| -----:|
| Full Text     | 100%| Yes | No | Yes | No | No |
| Native | 80%     | 100% | No | Yes | No | No |
| OCR | 30%      | 98% | No | Yes | No | Yes |

* An advantage of the Native method is that it also gets the text position while maintaining the accuracy of the FullText method.
* OCR uses 2 engines: Microsoft OCR is suitable for large images, while Google’s engine works better with smaller images and 
also provides a few more options like scale or invert.
* Data Scraping allows to extract structured data by pointing the first and second element we want to extract (and, when required, the link to the next page).
* We use Extract correlated data when more than 1 piece of information is needed from each element and Max Number Of Results to limit the amount of items we get.
