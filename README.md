# cloudmersive_nlp_api_client
The powerful Natural Language Processing APIs (v2) let you perform part of speech tagging, entity identification, sentence parsing, and much more to help you understand the meaning of unstructured text.

[Cloudmersive NLP API](https://www.cloudmersive.com/nlp-api) provides advanced machine learning-based natural language processing to detect language, sentiment, meaning and intent of text content.

- API version: v1
- Package version: 2.1.0


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

$apiInstance = new Swagger\Client\Api\AnalyticsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\HateSpeechAnalysisRequest(); // \Swagger\Client\Model\HateSpeechAnalysisRequest | Input hate speech analysis request

try {
    $result = $apiInstance->analyticsHateSpeech($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnalyticsApi->analyticsHateSpeech: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://api.cloudmersive.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AnalyticsApi* | [**analyticsHateSpeech**](docs/Api/AnalyticsApi.md#analyticshatespeech) | **POST** /nlp-v2/analytics/hate-speech | Perform Hate Speech Analysis and Detection on Text
*AnalyticsApi* | [**analyticsProfanity**](docs/Api/AnalyticsApi.md#analyticsprofanity) | **POST** /nlp-v2/analytics/profanity | Perform Profanity and Obscene Language Analysis and Detection on Text
*AnalyticsApi* | [**analyticsSentiment**](docs/Api/AnalyticsApi.md#analyticssentiment) | **POST** /nlp-v2/analytics/sentiment | Perform Sentiment Analysis and Classification on Text
*AnalyticsApi* | [**analyticsSimilarity**](docs/Api/AnalyticsApi.md#analyticssimilarity) | **POST** /nlp-v2/analytics/similarity | Perform Semantic Similarity Comparison of Two Strings
*AnalyticsApi* | [**analyticsSubjectivity**](docs/Api/AnalyticsApi.md#analyticssubjectivity) | **POST** /nlp-v2/analytics/subjectivity | Perform Subjectivity and Objectivity Analysis on Text
*ExtractEntitiesApi* | [**extractEntitiesPost**](docs/Api/ExtractEntitiesApi.md#extractentitiespost) | **POST** /nlp-v2/extract-entities | Extract entities from string
*LanguageDetectionApi* | [**languageDetectionGetLanguage**](docs/Api/LanguageDetectionApi.md#languagedetectiongetlanguage) | **POST** /nlp-v2/language/detect | Detect language of text
*LanguageTranslationApi* | [**languageTranslationTranslateDeuToEng**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslatedeutoeng) | **POST** /nlp-v2/translate/language/deu/to/eng | Translate German to English text with Deep Learning AI
*LanguageTranslationApi* | [**languageTranslationTranslateEngToDeu**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslateengtodeu) | **POST** /nlp-v2/translate/language/eng/to/deu | Translate English to German text with Deep Learning AI
*LanguageTranslationApi* | [**languageTranslationTranslateEngToFra**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslateengtofra) | **POST** /nlp-v2/translate/language/eng/to/fra | Translate English to French text with Deep Learning AI
*LanguageTranslationApi* | [**languageTranslationTranslateEngToRus**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslateengtorus) | **POST** /nlp-v2/translate/language/eng/to/rus | Translate English to Russian text with Deep Learning AI
*LanguageTranslationApi* | [**languageTranslationTranslateFraToEng**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslatefratoeng) | **POST** /nlp-v2/translate/language/fra/to/eng | Translate French to English text with Deep Learning AI
*LanguageTranslationApi* | [**languageTranslationTranslateRusToEng**](docs/Api/LanguageTranslationApi.md#languagetranslationtranslaterustoeng) | **POST** /nlp-v2/translate/language/rus/to/eng | Translate Russian to English text with Deep Learning AI
*ParseApi* | [**parseParseString**](docs/Api/ParseApi.md#parseparsestring) | **POST** /nlp-v2/parse/tree | Parse string to syntax tree
*PosTaggerApi* | [**posTaggerTagAdjectives**](docs/Api/PosTaggerApi.md#postaggertagadjectives) | **POST** /nlp-v2/pos/tag/adjectives | Part-of-speech tag a string, filter to adjectives
*PosTaggerApi* | [**posTaggerTagAdverbs**](docs/Api/PosTaggerApi.md#postaggertagadverbs) | **POST** /nlp-v2/pos/tag/adverbs | Part-of-speech tag a string, filter to adverbs
*PosTaggerApi* | [**posTaggerTagNouns**](docs/Api/PosTaggerApi.md#postaggertagnouns) | **POST** /nlp-v2/pos/tag/nouns | Part-of-speech tag a string, filter to nouns
*PosTaggerApi* | [**posTaggerTagPronouns**](docs/Api/PosTaggerApi.md#postaggertagpronouns) | **POST** /nlp-v2/pos/tag/pronouns | Part-of-speech tag a string, filter to pronouns
*PosTaggerApi* | [**posTaggerTagSentence**](docs/Api/PosTaggerApi.md#postaggertagsentence) | **POST** /nlp-v2/pos/tag/sentence | Part-of-speech tag a string
*PosTaggerApi* | [**posTaggerTagVerbs**](docs/Api/PosTaggerApi.md#postaggertagverbs) | **POST** /nlp-v2/pos/tag/verbs | Part-of-speech tag a string, filter to verbs
*RephraseApi* | [**rephraseEnglishRephraseSentenceBySentence**](docs/Api/RephraseApi.md#rephraseenglishrephrasesentencebysentence) | **POST** /nlp-v2/rephrase/rephrase/eng/by-sentence | Rephrase, paraphrase English text sentence-by-sentence using Deep Learning AI
*SegmentationApi* | [**segmentationGetSentences**](docs/Api/SegmentationApi.md#segmentationgetsentences) | **POST** /nlp-v2/segmentation/sentences | Extract sentences from string
*SegmentationApi* | [**segmentationGetWords**](docs/Api/SegmentationApi.md#segmentationgetwords) | **POST** /nlp-v2/segmentation/words | Get words in input string
*SpellcheckApi* | [**spellcheckCheckSentence**](docs/Api/SpellcheckApi.md#spellcheckchecksentence) | **POST** /nlp-v2/spellcheck/check/sentence | Check if sentence is spelled correctly
*SpellcheckApi* | [**spellcheckCorrectJson**](docs/Api/SpellcheckApi.md#spellcheckcorrectjson) | **POST** /nlp-v2/spellcheck/check/word | Find spelling corrections


## Documentation For Models

 - [CheckSentenceRequest](docs/Model/CheckSentenceRequest.md)
 - [CheckSentenceResponse](docs/Model/CheckSentenceResponse.md)
 - [CheckWordRequest](docs/Model/CheckWordRequest.md)
 - [CheckWordResponse](docs/Model/CheckWordResponse.md)
 - [CorrectWordInSentence](docs/Model/CorrectWordInSentence.md)
 - [Entity](docs/Model/Entity.md)
 - [ExtractEntitiesRequest](docs/Model/ExtractEntitiesRequest.md)
 - [ExtractEntitiesResponse](docs/Model/ExtractEntitiesResponse.md)
 - [GetWordsRequest](docs/Model/GetWordsRequest.md)
 - [GetWordsResponse](docs/Model/GetWordsResponse.md)
 - [HateSpeechAnalysisRequest](docs/Model/HateSpeechAnalysisRequest.md)
 - [HateSpeechAnalysisResponse](docs/Model/HateSpeechAnalysisResponse.md)
 - [LanguageDetectionRequest](docs/Model/LanguageDetectionRequest.md)
 - [LanguageDetectionResponse](docs/Model/LanguageDetectionResponse.md)
 - [LanguageTranslationRequest](docs/Model/LanguageTranslationRequest.md)
 - [LanguageTranslationResponse](docs/Model/LanguageTranslationResponse.md)
 - [ParseRequest](docs/Model/ParseRequest.md)
 - [ParseResponse](docs/Model/ParseResponse.md)
 - [PosRequest](docs/Model/PosRequest.md)
 - [PosResponse](docs/Model/PosResponse.md)
 - [PosSentence](docs/Model/PosSentence.md)
 - [PosTaggedWord](docs/Model/PosTaggedWord.md)
 - [ProfanityAnalysisRequest](docs/Model/ProfanityAnalysisRequest.md)
 - [ProfanityAnalysisResponse](docs/Model/ProfanityAnalysisResponse.md)
 - [RephraseRequest](docs/Model/RephraseRequest.md)
 - [RephraseResponse](docs/Model/RephraseResponse.md)
 - [RephrasedSentence](docs/Model/RephrasedSentence.md)
 - [RephrasedSentenceOption](docs/Model/RephrasedSentenceOption.md)
 - [SentenceSegmentationRequest](docs/Model/SentenceSegmentationRequest.md)
 - [SentenceSegmentationResponse](docs/Model/SentenceSegmentationResponse.md)
 - [SentimentAnalysisRequest](docs/Model/SentimentAnalysisRequest.md)
 - [SentimentAnalysisResponse](docs/Model/SentimentAnalysisResponse.md)
 - [SimilarityAnalysisRequest](docs/Model/SimilarityAnalysisRequest.md)
 - [SimilarityAnalysisResponse](docs/Model/SimilarityAnalysisResponse.md)
 - [SubjectivityAnalysisRequest](docs/Model/SubjectivityAnalysisRequest.md)
 - [SubjectivityAnalysisResponse](docs/Model/SubjectivityAnalysisResponse.md)
 - [WordPosition](docs/Model/WordPosition.md)


## Documentation For Authorization


## Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header


## Author




