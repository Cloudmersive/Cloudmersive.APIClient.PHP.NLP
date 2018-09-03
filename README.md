# cloudmersive_nlp_api_client
The powerful Natural Language Processing APIs let you perform part of speech tagging, entity identification, sentence parsing, and much more to help you understand the meaning of unstructured text.

[Cloudmersive NLP API](https://www.cloudmersive.com/nlp-api) provides advanced machine learning-based natural language processing to detect language, sentiment, meaning and intent of text content.

- API version: v1
- Package version: 1.3.9


## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/cloudmersive/cloudmersive_nlp_api_client.git"
    }
  ],
  "require": {
    "cloudmersive/cloudmersive_nlp_api_client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/cloudmersive_nlp_api_client/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\ExtractEntitiesStringApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = "value_example"; // string | Input string

try {
    $result = $apiInstance->extractEntitiesStringPost($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExtractEntitiesStringApi->extractEntitiesStringPost: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://api.cloudmersive.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ExtractEntitiesStringApi* | [**extractEntitiesStringPost**](docs/Api/ExtractEntitiesStringApi.md#extractentitiesstringpost) | **POST** /nlp/ExtractEntitiesString | Extract entities from string
*LanguageDetectionApi* | [**languageDetectionPost**](docs/Api/LanguageDetectionApi.md#languagedetectionpost) | **POST** /nlp/language/detect | Detect language of text
*ParseStringApi* | [**parseStringPost**](docs/Api/ParseStringApi.md#parsestringpost) | **POST** /nlp/ParseString | Parse string to syntax tree
*PosTaggerJsonApi* | [**posTaggerJsonPost**](docs/Api/PosTaggerJsonApi.md#postaggerjsonpost) | **POST** /nlp/PosTaggerJson | Part-of-speech tag a string
*PosTaggerStringApi* | [**posTaggerStringPost**](docs/Api/PosTaggerStringApi.md#postaggerstringpost) | **POST** /nlp/PosTaggerString | Part-of-speech tag a string
*SentencesApi* | [**sentencesPost**](docs/Api/SentencesApi.md#sentencespost) | **POST** /nlp/get/sentences/string | Extract sentences from string
*SpellCheckApi* | [**spellCheckCheckJson**](docs/Api/SpellCheckApi.md#spellcheckcheckjson) | **POST** /nlp/spellcheck/check/word/json | Spell check word
*SpellCheckApi* | [**spellCheckCheckSentenceJson**](docs/Api/SpellCheckApi.md#spellcheckchecksentencejson) | **POST** /nlp/spellcheck/check/sentence/json | Check if sentence is spelled correctly
*SpellCheckApi* | [**spellCheckCheckSentenceString**](docs/Api/SpellCheckApi.md#spellcheckchecksentencestring) | **POST** /nlp/spellcheck/check/sentence/string | Spell check a sentence
*SpellCheckApi* | [**spellCheckCorrect**](docs/Api/SpellCheckApi.md#spellcheckcorrect) | **POST** /nlp/spellcheck/correct/word/string | Find spelling corrections
*SpellCheckApi* | [**spellCheckCorrectJson**](docs/Api/SpellCheckApi.md#spellcheckcorrectjson) | **POST** /nlp/spellcheck/correct/word/json | Find spelling corrections
*SpellCheckApi* | [**spellCheckPost**](docs/Api/SpellCheckApi.md#spellcheckpost) | **POST** /nlp/spellcheck/check/word/string | Spell check a word
*WordsApi* | [**wordsAdjectives**](docs/Api/WordsApi.md#wordsadjectives) | **POST** /nlp/get/words/adjectives/string | Get adjectives in string
*WordsApi* | [**wordsAdverbs**](docs/Api/WordsApi.md#wordsadverbs) | **POST** /nlp/get/words/adverbs/string | Get adverbs in input string
*WordsApi* | [**wordsGetWordsJson**](docs/Api/WordsApi.md#wordsgetwordsjson) | **POST** /nlp/get/words/json | Get words in input string (JSON)
*WordsApi* | [**wordsGetWordsString**](docs/Api/WordsApi.md#wordsgetwordsstring) | **POST** /nlp/get/words/string | Get words from string
*WordsApi* | [**wordsNouns**](docs/Api/WordsApi.md#wordsnouns) | **POST** /nlp/get/words/nouns/string | Get nouns in string
*WordsApi* | [**wordsPost**](docs/Api/WordsApi.md#wordspost) | **POST** /nlp/get/words/verbs/string | Get the verbs in a string
*WordsApi* | [**wordsPronouns**](docs/Api/WordsApi.md#wordspronouns) | **POST** /nlp/get/words/pronouns/string | Returns all pronounts in string
*WordsApi* | [**wordsProperNouns**](docs/Api/WordsApi.md#wordspropernouns) | **POST** /nlp/get/words/properNouns/string | Get proper nouns in a string


## Documentation For Models

 - [CheckJsonResponse](docs/Model/CheckJsonResponse.md)
 - [CheckSentenceJsonResponse](docs/Model/CheckSentenceJsonResponse.md)
 - [CorrectJsonResponse](docs/Model/CorrectJsonResponse.md)
 - [CorrectWordInSentenceJsonResponse](docs/Model/CorrectWordInSentenceJsonResponse.md)
 - [GetWordsJsonResponse](docs/Model/GetWordsJsonResponse.md)
 - [LanguageDetectionResponse](docs/Model/LanguageDetectionResponse.md)
 - [PosRequest](docs/Model/PosRequest.md)
 - [PosResponse](docs/Model/PosResponse.md)
 - [PosSentence](docs/Model/PosSentence.md)
 - [PosTaggedWord](docs/Model/PosTaggedWord.md)
 - [WordPosition](docs/Model/WordPosition.md)


## Documentation For Authorization


## Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header


## Author



