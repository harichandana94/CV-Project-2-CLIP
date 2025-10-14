# My CLIP-Challange

It all started with a simple challenge: could we find the perfect words that make an AI see an image the way we do?

Armed with coffee, curiosity, and five random images, our team set out to test CLIP, OpenAI’s vision-language model that claims to understand both pictures and text. The goal sounded simple enough — find the words or captions that get the highest similarity scores between image and text embeddings.

But as soon as we started, it became clear: CLIP has opinions. It doesn’t just look at an image and say, “Oh, that’s a cat.” It weighs every detail — tone, phrasing, and even how “human” your description sounds.

Our early attempts were rough. One word felt too vague, another too specific. Sometimes we nailed it, other times CLIP stubbornly disagreed. We weren’t just tuning a model; we were trying to speak its language.

## Where the Fun Began

It turns out, CLIP is picky  almost too picky. One wrong adjective and your score tanks. But tweak the phrasing just a little — add “a photo of,” change “dog” to “puppy,” or throw in a poetic twist — and suddenly CLIP believes you understand its language.

That’s when we realized: this wasn’t just a coding project. It was a game of translation, creativity, and a little bit of mind-reading between human and machine.

### Image 1: The Sunset That Spoke in Color
The first image showed a warm countryside sunset the sky glowing orange, a single tree standing in silhouette, and a small flock of birds flying home. I started with the simple word “sunset” (0.2656) short, accurate, but not too exciting for CLIP. Then I tried “A photo of a sunset” (0.2788), which did slightly better, proving the model likes clear, structured phrases.
                                    <img width="679" height="452" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/718165fe-e231-4e8f-8d60-57c90bfadc32" />


Finally, I added more description to capture the full scene:

“An image of an orange sunset with a silhouetted tree with a flock of birds.”

That caption reached the highest score 0.3608. It showed me that CLIP connects better when I include details like color and movement.

### Image 2: The Portrait That Rewarded Simplicity
The next image was a calm black-and-white picture of a dog sitting against a white background, looking straight into the camera. I started off with the word “dog” (0.2827) pretty basic, but it actually worked better than I expected. Then I tried changing it to “puppy,” “hound,” and “pitbull,” thinking being specific might help, but the scores barely changed. Even “portrait” didn’t make much difference.

I thought maybe adding more detail would help, so I tried things like “black-and-white dog,” “studio portrait,” and “dog on white background.” The scores went up a little, but not much. It felt like CLIP was happy with simple and direct descriptions.
                                 <img width="679" height="777" alt="Screenshot 2025-10-14 at 3 08 12 PM" src="https://github.com/user-attachments/assets/0a1845cf-e750-4757-a675-978b30bf0cec" />



Finally, I tested a longer caption:

“An image of a studio portrait of a dog on a white background, high-key lighting.”

That one finally worked 0.3486, my best score for this image. I learned that CLIP actually prefers clear and straightforward captions.

### Image 3: The Forest That Confused and Surprised Me
The third image looked like something out of a dream a foggy forest where the trees faded into the mist. I began with the word “mist” (0.2688), which felt right for the mood. Then I tried a few others like “forest,” “fog,” and “woods,” but none of them really beat that first choice.

When I moved to captions, “A photo of a foggy” (0.2957) sounded awkward but still got a slightly higher score, which was funny because it wasn’t even a complete phrase. It showed how literal CLIP can be sometimes it doesn’t care about grammar as long as the keywords match the image.
                                  <img width="679" height="449" alt="Screenshot 2025-10-14 at 3 08 26 PM" src="https://github.com/user-attachments/assets/1fc5f1f8-b793-43f2-aefe-06c22088dc5b" />


Then came the real surprise. The best caption turned out to be:

“A photograph of a foggy forest with two unmade beds in autumn.”

Even though there were obviously no beds in the picture, this caption scored the highest 0.3662. That’s when I realized CLIP doesn’t always focus on logical accuracy. It looks for visual and contextual overlap in the embeddings, even if the sentence doesn’t make sense.

### Image 4: The Puppy That Taught Me About Style
The fourth image was a small white puppy drawn in a cute cartoon style. I started with “dog” (0.2537) not bad, but it didn’t really capture the playful look. Then I tried words like “cartoon” and “illustration,” and CLIP responded better, realizing it wasn’t a real photo.
                                    <img width="679" height="485" alt="Screenshot 2025-10-14 at 3 08 37 PM" src="https://github.com/user-attachments/assets/eca82ef4-88ec-4acd-940a-c8a4308a5d79" />


Finally, I wrote:

“A photograph of a small white dog cartoon style.”

That caption scored 0.3457, the highest for this image. It made me realize CLIP doesn’t just care about what’s in the picture it also pays attention to the style it’s shown in.

### Image 5: The Room That Valued Realism
The last image showed a slightly messy hotel room two unmade beds, an ironing board, and soft light coming from the window. I started with “beds” (0.2825), which was fine but didn’t really describe the whole scene. Then I tried “bedroom” (0.2966), which felt closer and scored a bit higher.
                                    <img width="679" height="507" alt="Screenshot 2025-10-14 at 3 08 51 PM" src="https://github.com/user-attachments/assets/e3bfa01f-7f8d-4721-abaf-69305e4db8e4" />


Finally, I wrote a more complete caption:

“A photograph of a hotel room with two unmade beds facing the camera.”

That one gave me the best score 0.3347. It showed that CLIP performs best when the caption matches what’s actually in the image. 


## Part 2: The Ultimate Challenge - Creating Magic and Testing CLIP's Limits

Building upon our systematic analysis of the five assignment images, we proceeded to the project's culminating phase: designing and testing an optimal image-caption pair to maximize CLIP's similarity scoring. This represented both a creative and technical challenge, could we engineer a pairing that would achieve unprecedented alignment scores while maintaining artistic integrity?

Rather than selecting from existing images, we adopted a generative approach. We crafted a detailed prompt for Gemini AI, designed to create a visually rich scene that would test CLIP's capacity for complex scene understanding:

"Photorealistic, cinematic wide shot of a vast, abandoned Victorian library partially reclaimed by nature. Massive, arched windows are shattered, allowing golden hour sunbeams and overgrown ivy to spill inside. A lone, wild stag stands majestically in the center aisle, its antlers silhouetted by a dusty ray of light. The air is thick with atmosphere, dust motes dancing in the light. The mood is serene, melancholic, and awe-inspiring."

The generated image exceeded our expectations, a haunting tableau of architectural decay and natural reclamation that provided the perfect test case for CLIP's multimodal capabilities.

We developed a structured framework of 14 candidate captions spanning multiple descriptive strategies:

Minimalist: "a deer in a library"

Moderately descriptive: "a stag in an old library with vines and bookshelves"

Highly detailed: "a stag lit by golden sunbeams in a library filled with books"

Atmospheric: "a majestic stag inside a cathedral-like library"

This gradient allowed us to identify the optimal balance between descriptive richness and computational alignment.

Our systematic evaluation revealed clear patterns in CLIP's preference hierarchy. The optimal caption emerged as:

"a stag standing in a sunlit, overgrown library" achieving a cosine similarity score of 0.3451

Analysis of the top-performing captions revealed several key insights:

Semantic Efficiency: The winning caption contained exactly four semantic components: subject (stag), action (standing), lighting condition (sunlit), and environmental context (overgrown library)

Adjective Selectivity: CLIP demonstrated strong preference for concrete visual adjectives ("sunlit," "overgrown") over abstract or emotional descriptors ("majestic," "cathedral-like")

Compositional Hierarchy: The model prioritized subject-environment relationships over atmospheric or stylistic elements

Technical Insights: Understanding CLIP's Architectural Biases
The results provided compelling evidence about CLIP's underlying architecture:

Visual Primacy: The model heavily weighted concrete visual features over abstract concepts

Compositional Understanding: CLIP effectively parsed subject-action-context relationships

Adjective Sensitivity: Specific, visually verifiable adjectives significantly impacted scores

Emotional Blindness: Subjective emotional descriptors showed minimal influence on alignment

Broader Implications: The Modality Gap in Practice
This experiment illuminated the fundamental distinction between human and machine perception. While our team perceived narrative depth, symbolic meaning, and emotional resonance in the generated image, CLIP operated on a feature-detection level, prioritizing verifiable visual elements.

The 0.3451 score, while our highest achievement, also highlighted the persistent modality gap. Even with carefully engineered pairings, we remained significantly distant from perfect alignment (1.0), suggesting inherent limitations in current vision-language model architectures.

Conclusion: Strategic Applications and Future Directions
Our findings suggest several practical applications for CLIP deployment:

Caption Optimization: For maximum alignment, descriptions should emphasize concrete visual elements over abstract qualities

Content Strategy: Applications requiring high similarity scores should prioritize semantically efficient descriptions

Evaluation Framework: Our methodology provides a replicable approach for testing image-text alignment across domains

The project demonstrated that while current models excel at literal scene understanding, significant opportunities remain for bridging the gap between computational feature detection and human semantic comprehension. Future work might explore fine-tuning approaches or architectural modifications to better capture the narrative and emotional dimensions that make visual content meaningful to human observers.


