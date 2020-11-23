# Google Spreadsheets phonetic transcription of English words
There is a formula for Google Spreadsheets to get the phonetic transcription of English word from Cambridge Dictionary.
International Phonetic Alphabet (IPA) symbols used.

```
=(JOIN("";IMPORTXML(CONCATENATE("https://dictionary.cambridge.org/dictionary/english/";A2);$C$2)))
```

*A2* -- the word you need to get transcription for

*C2* -- XPath to transcription element on the page of cambridge.org (it is a constant):

```
//*[@id="page-content"]/div[2]/div[1]/div[2]/div/div[3]/div/div/div/div[2]/span[1]/span[3]/span
```

![screenshot](https://raw.githubusercontent.com/OlegAnanyev/google-spreadsheets-phonetic-transcription/main/Screenshot_1.png)
