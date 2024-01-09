# Insightful Iris Experiments

## Using openAI's CustomGPTs

## CustomGPT Development
I've developed multiple CustomGPTs to represent different approaches in Prompt Engineering. In the first one, I worked more on creating a specific set of guidelines as single specific rules for image description; the second one took a more qualitative approach and classified those descriptions into tiers of preference. The third one is actually two CustomGPTs ... I split it into two different GPTs, one focused on just alt text, the other on the range of descriptions. This one leverages the first GPT with the guidelines and just changes the focus of the output. (I was curious if I split up the tasks if the result would be different — they are. Each set of texts get better. 

The different CustomGPTs can be found at the following URLs. (I've been calling them "Insightful Iris") You should be able to just drag an image into the text box and hit return to have it start producing results. Generally, they'll do it in table format because I wanted to make it easy to cut and paste into the Excel spreadsheet, but just ask it to produce paragraphs instead if you want it to be easier to read. 

- **Insightful Iris v1:** [Detailed Information](irisv1.md) | _[Iris v1 CustomGPT](https://chat.openai.com/g/g-whWygI1hy-insightful-iris-v1)_
- **Insightful Iris v2:** [Detailed Information](irisv2.md) | _[Iris v2 CustomGPT](https://chat.openai.com/g/g-P33BG6o5Z-insightful-iris-v2)_ 
- Insightful Iris, split into two specialized parts: [Detailed Information](irisv2.5.md)
	- **Alt Texter:** _[Alt Texter CustomGPT](https://chat.openai.com/g/g-3eqVFXPST-alt-texter-part-of-insightful-iris-v1)_
	- **Descriptive Art Narrator:** _[Descriptive Art Narrator CustomGPT](https://chat.openai.com/g/g-aFfyCbbNc-descriptive-art-narrator)_
- **Insightful Iris v3:** _coming_

I also have a handful of reference files to build the Knowledge of each CustomGPT. 

## Variations of Image Descriptions  
Realizing that there's substantial subjectivity and where biases inherent in the training set may come into play, in these longer form image descriptions, I've been creating three variations:

- **Straightforward, Factual:** At one end of a spectrum, this descriptions is close in tone and information to the original alt text, but in more detail. Ideally simply the characteristics of the artwork, the literal description of the physicality of the piece. 
	
- **Balanced:** A midpoint between the two endpoints, striking a balanced blend between raw information and the emotive experience. 
	
- **Emotional, Evocative:** At the other end of the spectrum, where expressive language is used to describe the emotional and affective experience of the object. When we "see" we don't simply see what's there, we're always interpreting it in some way. When a piece feels _moody_, that's a useful bit of information and part of the description. 
	
In practice, I can make cases for all three variations of the Image Description and that it will ultimately depend on the organizational voice and tone for the correct blend. I imagine a scoring mechanism supplied as part of the Instruction Set, such as _t=2_. This would be a midway blend between Straightforward (_t=1_) and Balanced (_t=3_) (and with Emotional as _t=5_). 
	
In the initial setup of the AI, I'd suggest doing an initial run of ~50 objects, getting all of the outputs, and in comparing all three, make a gut determination of what the desired tone value should be and then averaging out over the entire range of scores. There *is* going to be variability in tone across staff and different organizations. 

## Additional Notes
In the instruction sets, I've had better success with always having a defined persona / purpose for the GPT, offering clear instructions around the output, and providing both good and bad examples of output. I've been following some of the prompt research as of late, and I've happily paralleled a bunch of things that seem to lead to better success (although I've been doing multi-shot prompts and some other more advanced approaches, I'm not yet doing a medprompt style work, when I shift to the APIs, I think I can do that since there'll be more persistence to the AIs).

## Observations:

- There's an 8000 character limit to Instruction Sets, when adding lengthy rulesets / guidelines, that quickly can become an issue.
- I'm conflicted over the level of detail to provide in the accessibility guidelines. I've done both substantially shorter and longer ones. Longer ones don't appear to be better, but the shorter ones *do* seem to lose some detail. 
- If you're running in interactive mode (i.e. chatting, providing a single image at a time), the GPT can get lazy and start to provide shorter responses. Poking the GPT politely and asking it to double the length or asking how long something is supposed to be would correct it for some number of additional iterations.
- The CustomGPTs seem to get tired from time to time and start to trend to shorter outputs
- A handful of sessions have seen one of the GPTs periodically balk at some of the images — it indicates that it can't help with the image, although in every instance, I could just ask it to try again, and it gave the appropriate output
- The notion of word count is vague. For example, if I want descriptions that are around 175 words long, they'll range from 100 - 200 words, usually at the shorter end. However, if I ask to make it 30% longer, it does without any problem and will maintain the new approach for a while (until it starts to 'get tired’) 
- Different times of day seem to yield different results, and I suspect that has to do with the overall volume of use of OpenAI's system. 
- The GPTs do sometimes 'forget' parts of the instructions although when reminded or asked about it, they quickly correct. 
- There are a handful of errors in the descriptions, and I genuinely don't know where it gets the dimensions in some instances ... although when I confirm, it's usually pretty close. I've *only* been supplying images so maybe CMA's collection is part of the training; I have no idea nor any good way to validate if so. 

