# Accessibility / Image Description Discussion

## Multiple Kinds of Text
In general, for my purposes, I've been working from the idea that there are two kinds of texts that we're trying to create. While these can easily overlap, I'm teasing out a slight bit of distinction in order to flex our work in two different ways. 

- **Alt Text:** In which we're creating short descriptions for use as alt text for web images, social media, etc. Typically, these would be 2-3 sentences and narrowly factual. 
	
- **Image Descriptions:** These are substantially longer and more detailed, more in terms of a paragraph or two and can range from tons of factual information to starting to capture some of the affective and emotive experience of the artwork. 

	Realizing that there's substantial subjectivity and where biases inherent in the training set may come into play, in these longer form image descriptions, I've been creating three variations:

	- **Straightforward, Factual:** At one end of a spectrum, this descriptions is close in tone and information to the original alt text, but in more detail. Ideally simply the characteristics of the artwork, the literal description of the physicality of the piece. 
	
	- **Balanced:** A midpoint between the two endpoints, striking a balanced blend between raw information and the emotive experience. 
	
	- **Emotional, Evocative:** At the other end of the spectrum, where expressive language is used to describe the emotional and affective experience of the object. When we "see" we don't simply see what's there, we're always interpreting it in some way. When a piece feels _moody_, that's a useful bit of information and part of the description. 
	
	In practice, I can make cases for all three variations of the Image Description and that it will ultimately depend on the organizational voice and tone for the correct blend. I imagine a scoring mechanism supplied as part of the Instruction Set, such as _t=2_. This would be a midway blend between Straightforward (_t=1_) and Balanced (_t=3_) (and with Emotional as _t=5_). 
	
	In the initial setup of the AI, I'd suggest doing an initial run of ~50 objects, getting all of the outputs, and in comparing all three, make a gut determination of what the desired tone value should be and then averaging out over the entire range of scores. There *is* going to be variability in tone across staff and different organizations. 

## Rules for Image descriptions
There is a plethora of information around best practices in describing images. I pulled from multiple sources across the web including:

- _links to web resources here_

And, in turn fed this into a CustomGPT that was configured as an accessibility expert to extract the following, which, based on personal experience, seem to cover a pretty broad spectrum of things I've experienced in parts and pieces. These have broken into three tiers of priority, to give some sense of overall order and important. 

- **Tier 1: Most Critical Elements**

	1. Main Subject and Action: Describe the central figure or focus of the image and any significant action or activity taking place.  
	_Example: "A man is jogging along a beach at sunrise. Seagulls are flying low near the water's edge."__

	2. Composition and Layout: Explain the arrangement of elements within the image, including their relative positions and relationships.  
	_Example: "The photo captures a bustling city street with tall buildings on either side, framing a busy pedestrian crosswalk in the center."__

	3. Dominant Colors and Materials (Artworks): For artworks, specify the primary colors and materials used, emphasizing their prominence and interaction.  
	_Example: "The oil painting features deep blues and vibrant greens, depicting a nighttime landscape with trees and a starry sky."__

	4. Text in Images: If there is text within the image, read and describe it, explaining its relevance to the overall image.  
	_Example: "A street sign in the foreground reads ‘Broadway,’ set against a backdrop of crowded sidewalks and bright city lights."__

	5. Mood or Tone: Convey the overall emotional feel or atmosphere of the image, highlighting how the visual elements contribute to this mood.  
	_Example: "The portrait conveys a sense of solemnity, with the subject's serious expression against a dark, muted background."__

	6. Element Placement and Position: Describe where key elements are situated within the image and their orientation to one another.  
	_Example: "In the center of the painting, a large oak tree stands tall, with a small cottage nestled to its right, partially obscured by shadows."__

- **Tier 2: Important but Secondary Elements**

	7. Background Details: Describe significant elements in the background that add context or depth to the image.  
	_Example: "Behind the main scene of a picnic, there's a lake with ducks and a distant row of trees under a cloudy sky."__

	8. Texture and Material Detailing (Artworks): For artworks, mention and describe the material composition and textures, giving a sense of the physical qualities.  
	_Example: "The sculpture is made of rough, weathered bronze, with intricate patterns etched into its surface."__

	9. Color and Pattern Description: Describe the colors and patterns present in the image, and how they interact with each other.  
	_Example: "The quilt in the image has a patchwork of reds, blues, and yellows in a checkered pattern, creating a vibrant and homely feel."__

	10. Lighting and Shadow: Note how light and shadow are used in the image, particularly in artworks, to create depth or focus.  
	_Example: "Sunlight filters through the window, casting long shadows on the wooden floor and highlighting the dust in the air."__

	11. Detail Visibility Notation: Point out subtle or easily missed details in the image, especially those that might not be immediately apparent.  
	_Example: "In the lower right corner, a small inscription is barely visible on the stone wall."__

	12. Emotional and Symbolic Attributes (Artworks): Include and objectively describe emotional or symbolic aspects of artworks, conveying deeper meanings and feelings.  
	_Example: "The painting's somber blues and isolated figure on the bridge evoke a feeling of loneliness and introspection."__

	13. Movement and Energy Conveyance: Convey any sense of motion or vitality present in the image, depicting dynamic elements.  
	_Example: "The photograph captures a dancer in mid-twirl, her skirt fanning out around her in a blur of motion."__

	14. Narrative Element Visualization: Visually describe storytelling elements within the image, bringing any narrative aspects to life.  
	_Example: "The mural depicts a bustling marketplace scene, with vendors and shoppers interacting, suggesting a lively community atmosphere."__

	15. Setting and Emotional Impact Description: Describe the setting of the image and its impact on the overall emotional tone.  
	_Example: "The abandoned house, with its peeling paint and overgrown garden, creates a feeling of desolation and neglect."__

- **Tier 3: Supplementary Details**

	16. Historical or Cultural Context (Artworks): Provide any relevant historical or cultural background that enhances understanding of the artwork.  
	_Example: "This 18th-century landscape painting reflects the Romantic era's fascination with nature and emotion, evident in its dramatic portrayal of a stormy sea."__

	17. Unique or Unusual Features: Highlight any features of the image that are particularly distinctive or uncommon.  
	_Example: "In this wildlife photo, a rare albino deer is seen standing out against a dark forest backdrop."__

	18. Perspective and Viewpoint: Describe the angle or perspective from which the image is taken or portrayed.  
	_Example: "The aerial photograph captures the city from above, presenting a maze-like view of streets and buildings."__

	19. Scale and Proportion: Mention if elements are exaggerated, minimized, or life-sized, particularly in artworks.  
	_Example: "The statue is a colossal representation of a human figure, towering over its surroundings at twice life size."__

	20. Frame or Borders (Artworks): Describe the frame or border of an artwork if it contributes to the understanding or aesthetic of the piece.  
	_Example: "The painting is set in an ornate, gilded frame that adds to its classical elegance."__

	21. Artist's Signature or Markings: Mention the artist's signature or any unique markings, if visible.  
	_Example: "The artist's signature, a small red stamp, is subtly placed in the bottom left corner of the canvas."__

	22. Descriptive Metaphors: Use metaphors to describe abstract aspects of the image, aiding in interpretation.  
	_Example: "The swirls in the sky of the painting resemble a tumultuous sea, mirroring the emotional turmoil depicted."__

	23. Element Interaction Explanation: Explain how different elements within the image interact or relate to each other.  
	_Example: "The shadows of the trees in the foreground create a contrast with the brightly lit meadow in the background, adding depth."__

	24. Contextual Element Description: Describe elements in relation to each other to provide context and show interconnectedness.  
	_Example: "The small figure in the corner of the mural is overshadowed by the massive urban skyline, emphasizing the theme of nature versus urbanization."__

	25. Textural Quality Highlighting (Artworks): Highlight texture and material quality in artworks, providing a tactile sense of surfaces.  
	_Example: "The impasto technique in the painting gives the flower petals a three-dimensional, almost touchable quality."__

	26. Specificity in Decorative Details: Be specific about decorative aspects of the image, detailing their appearance and contribution to the overall image.  
	_Example: "The intricate border of the manuscript page features gold leaf and vivid blue miniature flowers."__

	27. Cultural and Functional Context Inclusion: Include relevant cultural or functional context to enhance understanding of the image.  
	_Example: "This traditional Japanese woodblock print, used historically for storytelling, depicts a famous scene from folklore."__

	28. Style and Technique Description (Artworks): Describe the style and techniques used by the artist, highlighting their method and approach.  
	_Example: "The artist employs a pointillism technique, creating the image from thousands of small, distinct dots of color."__

	29. Medium Specificity: Specify the medium used in artworks, providing insight into the materials and methods employed.  
	_Example: "This mixed media piece combines acrylics with collage elements, creating a layered and textured effect."__

	30. Contextual Background Provision: Provide historical or cultural background information for better understanding of the image's significance.  
	_Example: "The photograph, taken during the early 20th century, captures the essence of the industrial era with its focus on factory workers."__

	31. Iconography and Imagery Explanation: Explain imagery and iconography present in the image, particularly in artworks, interpreting symbolic and representational elements.  
	_Example: "The mural's central figure, a dove, symbolizes peace amidst the surrounding chaos of abstract shapes."__

	32. Skin Tones and Representation Mention: Mention skin tones and racial identities where relevant, avoiding assumptions and ensuring diverse representation.  
	_Example: "The portrait gallery features a diverse range of subjects, from fair to deep skin tones, representing various ethnicities."__

	33. Use of Familiar Terms and Colors: Use common color names and avoid technical jargon, making the description accessible and understandable.  
	_Example: "The sky in the painting transitions from a deep navy to a soft baby blue, mimicking a real sunset."__

	34. Universal Color Descriptions: Describe colors in universally understandable terms, ensuring clarity and inclusivity for all audiences.  
	_Example: "The fabric's colors range from sunflower yellow to ocean blue, with splashes of crimson red."__

	35. Sensory Inclusion in Descriptions: Offer descriptions that engage multiple senses, providing a richer, more engaging experience.  
	_Example: "The sound of the waterfall in the photograph seems almost audible, complemented by the vivid greens and blues of the surrounding foliage."__

	36. Directional Language Utilization: Use directional language to aid in understanding the composition, clarifying the arrangement and orientation of elements.  
	_Example: "From the top left to the bottom right of the canvas, a river snakes through the landscape, guiding the viewer's eye."__

	37. Logical Description Organization: Organize the description coherently, ensuring a logical flow that enhances understanding.  
	_Example: "Starting from the foreground with detailed flowers and moving to the misty mountains in the background, the painting takes the viewer on a visual journey."__

	38. Structural Consistency Maintenance: Maintain a predictable and consistent structure in descriptions, aiding clarity and comprehension.  
	_Example: "Each segment of the triptych features a different season, presented in a consistent style with a central tree changing from green to gold to bare."__

	39. Simplicity in Language: Use straightforward language, avoiding complexity to ensure accessibility for all listeners.  
	_Example: "The child's drawing shows a simple house with a triangular roof, square windows, and a round door."__

	40. Conciseness and Clarity in Descriptions: Be succinct yet comprehensive, providing detailed descriptions without unnecessary verbosity.  
	_Example: "The map is clearly marked with major cities in bold, connected by red lines representing highways."__

	41. Avoidance of Curatorial Interpretation: Focus on the visual aspects of the artwork, avoiding subjective interpretation or analysis.  
	_Example: "The abstract painting consists of geometric shapes in primary colors, without suggesting any specific meaning."_

	42. Jargon Avoidance: Use simple language and explain any technical terms, ensuring accessibility to all viewers.  
	_Example: "The fresco, a type of mural painted on wet plaster, shows a scene from Roman mythology."__

	43. Clarification of Unusual Terms: Briefly explain specific art terms used, aiding in understanding for those unfamiliar with art terminology.  
	_Example: "Chiaroscuro, a technique involving strong contrasts between light and dark, is used to give depth to the figures in the painting."__

	44. Ambiguity Avoidance: Use specific and clear language, avoiding vague or ambiguous descriptions.  
	_Example: "The sculpture is a realistic depiction of a human hand, about 18 inches in length, with detailed fingers and palm lines."__

	45. Over-Interpretation Avoidance: Stick to visible elements, avoiding assumptions or extensive interpretation beyond what is evident.  
	_Example: "The landscape painting shows rolling hills and a river, without implying any particular season or time of day."__

	46. Repetition Avoidance: Add new details beyond what is provided in titles or captions, offering additional insights.  
	_Example: "Although titled ‘Sunset Over the Mountains,’ the painting also features a small cabin and a campfire in the foreground, adding to the scene."__

	47. Non-Visual Detailing: Describe braille or tactile features if present, catering to viewers with vision impairments.  
	_Example: "The exhibit includes a tactile model of the sculpture, allowing visitors to feel its contours and shapes."__

	48. Inclusivity in Descriptions: Ensure descriptions are accessible and understandable to a broad audience, considering diverse needs and backgrounds.  
	_Example: "The children's book illustration is colorful and simple, featuring animals that are easily recognizable, like a smiling cat and a hopping rabbit."__

	49. Symbolic/Iconic Element Visualization: Visually describe symbolic or iconic elements, aiding in understanding their significance.  
	_Example: "The flag in the painting, with its stars and stripes, symbolizes national pride amidst the historical scene depicted."__

	50. Contrast and Composition Emphasis: Emphasize contrasts and composition styles, highlighting these aspects for a deeper appreciation.  
	_Example: "The black-and-white photograph emphasizes the contrast between the illuminated skyscrapers and the dark night sky."__

	51. Text Transcription Inclusion: Include a transcription of any visible text without repetition, providing context and additional information.  
	_Example: "The bottom of the poster includes small text: ‘Event sponsored by the City Arts Council, open to all.’”__
