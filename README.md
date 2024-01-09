# Advanced Prompt Engineering Comparisons
A comparison of different advanced prompt engineering techniques as applied to image descriptions of artworks for the museum field.
_maintained by Bruce Wyman / bwyman@usd-mach.com_
_last updated: Jan 8, 2024_

This repository establishes a set of guidelines for creating accessibile image descriptions for artworks, a detailed comparison of different Prompt Engineering Techniques, and early experiments at implementation. 

**Pending Tasks:**

- [ ] Add Intro to main README.md
- [ ] Add narrative to each [Iris experiment](experiments/insightfuliris.md)
- [ ] Create generic examples for each of the [prompt techniques](prompts/techniques.md)
- [ ] Create Iris Instruction set & sample responses for each prompt technique

## Menu:

- **Background**
	- [Accessibility Rules](accessibility/accessibility_rules.md)
	- [Prompt Engineering Techniques](prompts/techniques.md)

- **Experiments**
	- [Insightful Iris Experiments](experiments/insightfuliris.md)
	
- **Useful Onnline Resources**
	- [Principled Instructions Are All You Need for Questioning LLaMA-1/2, GPT-3.5/4](https://arxiv.org/pdf/2312.16171v1.pdf?utm_source=www.theneurondaily.com&utm_medium=newsletter&utm_campaign=26-prompting-hacks)
	- [The Power of Prompting](https://www.microsoft.com/en-us/research/blog/the-power-of-prompting/)
	- [Steering at the Frontier](https://www.microsoft.com/en-us/research/blog/steering-at-the-frontier-extending-the-power-of-prompting/)
	- [OpenAI's Prompting Guide](https://platform.openai.com/docs/guides/prompt-engineering)

Based on this collected information, it's definitely possible to get fairly detailed, low hallucination results using a CustomGPT approach with a refined instruction set and basic set of knowledge.

For example, for Cleveland Museum of Art's [_The Biglin Brothers Turning The Stake_](https://www.clevelandart.org/art/1927.1984), it's possible to get something fairly detailed (this is from the CustomGPT, Insightful Iris v3):

>This oil painting, rendered with a realistic attention to detail, measures approximately 56 by 86 centimeters. It presents a serene riverscape scene, centered on two male rowers in a slender racing shell, which is depicted with a glossy, reddish-brown hue that reflects the calm water. The athletes, dressed in white sleeveless tops and dark shorts, exhibit physical exertion as suggested by their well-defined arm muscles and concentrated facial expressions. Both wear blue bandanas, which add a vibrant splash of color in contrast to their otherwise muted attire.

>The rowers are positioned slightly off-center to the left, allowing the viewer's eye to wander towards the right where a tall flagpole stands erect with a deep blue flag that flutters softly in the air, injecting verticality and a sense of motion into the composition. The water is rendered with subtle gradations of blue and gray, mirroring the overcast sky above, which is painted in soft whites and grays, suggesting a diffuse light source.

>In the background, the distant shore is alive with minute figures of spectators, rendered in earthy tones that blend with the greenery of the trees. Their presence adds a communal atmosphere to the scene. The right background features a vintage steamboat with a slender plume of smoke rising into the sky, suggesting the early industrial era and leisurely river activities. The artist's use of light and shadow on the water's surface creates a sense of depth, while the reflections of the rowers and the flag underscore the painting's tranquil ambiance.

And these outputs work across a wide range of images, including this image of [Tintin on the Moon](https://cdn001.tintin.com/public/tintin/img/static/explorers-on-the-moon/C16_Marche-en-p25-bcd%20color.png):

>This illustration, drawn in a comic book style, features a bold scene of lunar exploration. Dominating the image is a large rocket with a red-and-white checkered pattern, standing upright on the moon. The rocket's design is reminiscent of mid-20th-century space race aesthetics, with a pointed nose cone, cylindrical body, and three large fins providing stability. The landscape is rendered in a monochromatic greenish-gray, textured to depict the rough and pockmarked lunar surface filled with various-sized craters.

>In stark contrast to the immensity of the rocket, a small astronaut is depicted in the foreground. The astronaut's suit is detailed, with a classic design that includes a bulky life-support backpack, helmet, and visor. The figure's pose captures a moment of triumph and awe as they step onto the moon's surface. A speech bubble emerges from the astronaut, containing a text that underscores the historic nature of the event being depicted. The background consists of a stark, black sky and a distant mountain range, adding to the desolation and grandeur of the lunar environment.