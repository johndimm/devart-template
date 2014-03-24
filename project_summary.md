# TalkShow

story illustrator

## Authors
- John Dimm, [johndimm](https://github.com/johndimm)


## Description
TalkShow eavesdrops on conversations, converting overheard speech to text, and using the text to search for relevant images on the internet. The gallery installation would have an open microphone on a stand in front of a video wall consisting of four large flat screen televisions.

## Link to Prototype

[TalkShow](https://dprhcp108.doteasy.com/~johndimm/TalkShow/)

## Example Code

<pre>
  [from speech.js]
  // The final transcript has the words that we're sure about.
  // The interim transcript has a hypothesis that may change.
  var interim_transcript = '';  
  for (var i = event.resultIndex; i < event.results.length; ++i) {
    if (event.results[i].isFinal) {
      g_finalTranscript += event.results[i][0].transcript;
    } else {
      interim_transcript += event.results[i][0].transcript;
    }
  }
</pre>

## Links to External Libraries

- [Web Speech API](https://dvcs.w3.org/hg/speech-api/raw-file/tip/speechapi.html) for speech recognition
- [flickr api](http://www.flickr.com/services/api/) for image search
- [bing search api](http://datamarket.azure.com/dataset/bing/search) for image search
- [alchemy api](http://www.alchemyapi.com/api/entity/langs.html) for named entity recognition



## Images & Videos


[YouTube video demo in French](https://www.youtube.com/watch?v=j0BDSlrP63Q)


