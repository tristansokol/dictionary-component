#dictionary-component
*A google polymer web component set for the Longman Dictionary API*
***

This is an example web component that uses the [Longman Dictonary API](https://developer.pearson.com/apis/dictionaries/) for use with [Google Polymer](http://www.polymer-project.org/)

All of the elements can be demoed on the index.html page. This app uses the sandbox API key, so fuctionality is limited (mostly to words starting with a, b, or c) you can apply for your own key to use on the [Longman Dictonary API](https://developer.pearson.com/apis/dictionaries/) page. 

See a demo at http://tristansokol.com/dict/

##Components:

###Basic Definition

```
<longman-basic-definition apikey="" word="">

```
Displays the first definition of *word* 
***
###Synonyms

```
<longman-synonyms apikey="" word="">

```
Displays the first few synonyms and defintions of *word* 
***
###Related Words

```
<longman-related-words apikey="" word="">

```
Displays the a couple words related to *word* and their definition
***
###Get Definition

```
<longman-get-definition word=""  apikey="" definitionJson related synonyms">

```
This is a behind the scenes support element used in the other elements to actually interact with the Longman API.

**definitionJson** returns the results of the API to be displayed by the other elements

**related** is to be set if you want to look up related words instead of the default of a definition. Same for **synonyms**

***

