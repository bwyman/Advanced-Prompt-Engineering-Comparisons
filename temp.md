
# Variations of Image Descriptions  
Realizing that there's substantial subjectivity and where biases inherent in the training set may come into play, in these longer form image descriptions, I've been creating three variations:

- **Straightforward, Factual:** At one end of a spectrum, this descriptions is close in tone and information to the original alt text, but in more detail. Ideally simply the characteristics of the artwork, the literal description of the physicality of the piece. 
	
- **Balanced:** A midpoint between the two endpoints, striking a balanced blend between raw information and the emotive experience. 
	
- **Emotional, Evocative:** At the other end of the spectrum, where expressive language is used to describe the emotional and affective experience of the object. When we "see" we don't simply see what's there, we're always interpreting it in some way. When a piece feels _moody_, that's a useful bit of information and part of the description. 
	
In practice, I can make cases for all three variations of the Image Description and that it will ultimately depend on the organizational voice and tone for the correct blend. I imagine a scoring mechanism supplied as part of the Instruction Set, such as _t=2_. This would be a midway blend between Straightforward (_t=1_) and Balanced (_t=3_) (and with Emotional as _t=5_). 
	
In the initial setup of the AI, I'd suggest doing an initial run of ~50 objects, getting all of the outputs, and in comparing all three, make a gut determination of what the desired tone value should be and then averaging out over the entire range of scores. There *is* going to be variability in tone across staff and different organizations. 
