# My CLIP-Challange

## The Spark of Curiosity
It all started with a simple challenge: could we find the perfect words that make an AI see an image the way we do?

Armed with coffee, curiosity, and five random images, our team set out to test CLIP, OpenAI’s vision-language model that claims to understand both pictures and text. The goal sounded simple enough find the words or captions that get the highest similarity scores between image and text embeddings.

But as soon as we started, it became clear: CLIP has opinions. It doesn’t just look at an image and say, “Oh, that’s a cat.” It weighs every detail, tone, phrasing, and even how “human” your description sounds.

Our early attempts were rough. One word felt too vague, another too specific. Sometimes we nailed it, other times CLIP stubbornly disagreed. We weren’t just tuning a model; we were trying to speak its language.

## The Early Struggles

Initially, our attempts were met with mixed results. One word felt too vague, another too specific. Sometimes we nailed it, other times CLIP stubbornly disagreed. We weren't just tuning a model; we were trying to speak its language.

## Where the Fun Began

It turns out, CLIP is picky  almost too picky. One wrong adjective and your score tanks. But tweak the phrasing just a little, add “a photo of,” change “dog” to “puppy,” or throw in a poetic twist, and suddenly CLIP believes you understand its language.

That’s when we realized: this wasn’t just a coding project. It was a game of translation, creativity, and a little bit of mind-reading between human and machine.

### Image 1: The Sunset That Spoke in Color
The first image showed a warm countryside sunset the sky glowing orange, a single tree standing in silhouette, and a small flock of birds flying home. I started with the simple word “sunset” (0.2656) short, accurate, but not too exciting for CLIP. Then I tried “A photo of a sunset” (0.2788), which did slightly better, proving the model likes clear, structured phrases.
<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/718165fe-e231-4e8f-8d60-57c90bfadc32" />
</p>
<p align="center">
  <a href="https://images.pexels.com/photos/36744/agriculture-arable-clouds-countryside.jpg">Image Link</a>
</p>


Finally, I added more description to capture the full scene: 

“An image of an orange sunset with a silhouetted tree with a flock of birds.”

That caption reached the highest score 0.3608. It showed me that CLIP connects better when I include details like color and movement.

### Image 2: The Portrait That Rewarded Simplicity
The next image was a calm black-and-white picture of a dog sitting against a white background, looking straight into the camera. I started off with the word “dog” (0.2827) pretty basic, but it actually worked better than I expected. Then I tried changing it to “puppy,” “hound,” and “pitbull,” thinking being specific might help, but the scores barely changed. Even “portrait” didn’t make much difference.

I thought maybe adding more detail would help, so I tried things like “black-and-white dog,” “studio portrait,” and “dog on white background.” The scores went up a little, but not much. It felt like CLIP was happy with simple and direct descriptions.
<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/0a1845cf-e750-4757-a675-978b30bf0cec" />
  <p align="center">
  <a href="https://images.pexels.com/photos/825947/pexels-photo-825947.jpeg">Image Link</a>
</p>




Finally, I tested a longer caption:

“An image of a studio portrait of a dog on a white background, high-key lighting.”

That one finally worked 0.3486, my best score for this image. I learned that CLIP actually prefers clear and straightforward captions.

### Image 3: The Forest That Confused and Surprised Me
The third image looked like something out of a dream a foggy forest where the trees faded into the mist. I began with the word “mist” (0.2688), which felt right for the mood. Then I tried a few others like “forest,” “fog,” and “woods,” but none of them really beat that first choice.

When I moved to captions, “A photo of a foggy” (0.2957) sounded awkward but still got a slightly higher score, which was funny because it wasn’t even a complete phrase. It showed how literal CLIP can be sometimes it doesn’t care about grammar as long as the keywords match the image.
<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/1fc5f1f8-b793-43f2-aefe-06c22088dc5b" />
  <p align="center">
  <a href="https://images.pexels.com/photos/34044163/pexels-photo-34044163.jpeg">Image Link</a>
</p>




Then came the real surprise. The best caption turned out to be:

“A photograph of a foggy forest with two unmade beds in autumn.”

Even though there were obviously no beds in the picture, this caption scored the highest 0.3662. That’s when I realized CLIP doesn’t always focus on logical accuracy. It looks for visual and contextual overlap in the embeddings, even if the sentence doesn’t make sense.

### Image 4: The Puppy That Taught Me About Style
The fourth image was a small white puppy drawn in a cute cartoon style. I started with “dog” (0.2537) not bad, but it didn’t really capture the playful look. Then I tried words like “cartoon” and “illustration,” and CLIP responded better, realizing it wasn’t a real photo.
<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/eca82ef4-88ec-4acd-940a-c8a4308a5d79" />
</p>
 <p align="center">
  <a href="https://live.staticflickr.com/840/43380549381_004601c7ac_h.jpg">Image Link</a>
</p>

Finally, I wrote:

“A photograph of a small white dog cartoon style.”

That caption scored 0.3457, the highest for this image. It made me realize CLIP doesn’t just care about what’s in the picture it also pays attention to the style it’s shown in.

### Image 5: The Room That Valued Realism
The last image showed a slightly messy hotel room two unmade beds, an ironing board, and soft light coming from the window. I started with “beds” (0.2825), which was fine but didn’t really describe the whole scene. Then I tried “bedroom” (0.2966), which felt closer and scored a bit higher.
<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/e3bfa01f-7f8d-4721-abaf-69305e4db8e4" />
</p>
 <p align="center">
  <a href="https://live.staticflickr.com/2404/2020522557_d1aa0a1066_k.jpg">Image Link</a>
</p>

Finally, I wrote a more complete caption:

“A photograph of a hotel room with two unmade beds facing the camera.”

That one gave me the best score 0.3347. It showed that CLIP performs best when the caption matches what’s actually in the image. 


## Part 2: The Ultimate Challenge - Creating Magic and Testing CLIP's Limits

Building upon our systematic analysis of the five assignment images, we moved into the project’s culminating phase: designing and testing an optimal image–caption pair to push CLIP’s similarity scoring to its limits.
This was both a creative and a technical pursuit, could we engineer a pairing that achieved unprecedented alignment while preserving artistic integrity?

### The Generative Experiment

Rather than using existing imagery, we adopted a generative approach.
Using Gemini AI, we crafted a detailed text-to-image prompt designed to test CLIP’s ability to interpret complex, cinematic scenes:

“Photorealistic, cinematic wide shot of a vast, abandoned Victorian library partially reclaimed by nature.
Massive arched windows are shattered, letting golden-hour sunbeams and ivy spill inside.
A lone stag stands majestically in the center aisle, its antlers silhouetted by a dusty ray of light.
The mood is serene, melancholic, and awe-inspiring.”

The generated image exceeded our expectations — a haunting tableau of architectural decay and natural reclamation.
It provided an ideal test case for evaluating CLIP’s multimodal understanding: could the model connect this deeply atmospheric visual to equally rich textual descriptions?
### Caption Framework & Evaluation

We developed a structured framework of 14 candidate captions, arranged along a descriptive gradient:
| Type                     | Example                                                        |
| ------------------------ | -------------------------------------------------------------- |
| *Minimalist*             | “a deer in a library”                                          |
| *Moderately descriptive* | “a stag in an old library with vines and bookshelves”          |
| *Highly detailed*        | “a stag lit by golden sunbeams in a library filled with books” |
| *Atmospheric*            | “a majestic stag inside a cathedral-like library”              |


<p align="center">
  <img width="500" height="500" alt="" src="mygeneratedimage.png" />
  <br>
  <em>This image was generated by ChatGPT 5 </em>
</p>




This progression allowed us to examine how caption complexity affects CLIP’s embedding alignment and identify the balance point between descriptiveness and semantic precision.

### The Winning Pair

Our systematic evaluation produced clear results.
The optimal caption was:

“a stag standing in a sunlit, overgrown library”
Cosine similarity = 0.3451

This caption achieved the highest score among all candidates.

Why it worked:

- Semantic efficiency: the caption contained exactly four semantic components: subject (stag), action (standing), lighting (sunlit), environment (overgrown library)

- Adjective selectivity: CLIP favored concrete visual adjectives (“sunlit,” “overgrown”) over abstract ones (“majestic,” “cathedral-like”).

- Compositional hierarchy: the model prioritized subject + environment relationships above mood or stylistic tone.

### Technical Insights: Understanding CLIP’s Architectural Biases

Our results offered valuable evidence about CLIP’s internal weighting and limitations:

- Visual Primacy: CLIP relies heavily on visually verifiable features, not narrative or emotion.

- Compositional Understanding: the model captured subject–action–context structure with notable precision.

- Adjective Sensitivity: specific, image-grounded modifiers significantly increased similarity scores.

- Emotional Blindness: words expressing mood or symbolism contributed little to alignment.

### The Modality Gap in Practice

This experiment vividly illustrated the modality gap — the representational divide between human perception and machine reasoning.
While humans perceived the image as symbolic and emotionally rich, CLIP operated strictly on feature detection, rewarding what it could see rather than what it could feel.

Even with an engineered, semantically perfect pairing, our top similarity score of 0.3451 remained far from 1.0, underscoring the persistent limitations of current vision-language models.


### Our Learnings

After diving deep into CLIP with five very different images and pushing it to its limits, here’s what stood out to us:

**CLIP is extremely literal.** It rewarded captions that described exactly what was visible in the image. Poetic phrasing, mood words, or abstract ideas didn’t improve scores.

**Details matter, but the right ones.** Adding color, lighting, and spatial relationships consistently boosted similarity, while extra adjectives that weren’t visually grounded often didn’t help.

**Style influences perception.** CLIP can tell the difference between a photo, illustration, or cartoon, and captions that matched the image’s style scored higher.

**Longer doesn’t always mean better, but precise counts.** Concise, semantically efficient captions describing the subject, action, environment, and lighting outperformed both overly brief and overly flowery ones.

**Generative AI is a strong ally.** Using tools like Gemini to create captions often matched or exceeded our manual attempts, showing that AI can understand visual semantics surprisingly well.

**There’s a ceiling.** Even our best-engineered captions reached only around 0.345. This demonstrates the modality gap: CLIP can measure visual similarity but can’t fully capture human perception or the emotional “story” of an image.

**Context and composition are key.** Captions that clearly reflected relationships between objects, the environment, and light consistently did better than those that focused on mood or abstract concepts.

### Conclusion — Applications & Future Directions

Our findings point to practical strategies for improving real-world CLIP performance:

- Caption Optimization: use concise, visually grounded descriptions; avoid subjective emotion words.

- Content Strategy: for tasks like image retrieval or classification, prioritize semantic efficiency over poetic language.

- Evaluation Framework: our method provides a replicable pipeline for assessing image–text alignment across domains.

Ultimately, our project showed that CLIP excels at literal scene comprehension, yet struggles with emotional or symbolic nuance.
Bridging this gap will require future models that integrate visual grounding with affective and contextual reasoning, enabling AI systems to perceive images not only as patterns of pixels — but as stories worth understanding.







