# My CLIP-Challange When AI Sees Differently Than We Do

## The Spark of Curiosity

The Day We Started Speaking CLIP's Language
It began with what seemed like a straightforward task: find the perfect words that make an AI understand images the way humans do. Little did we know we were about to become translators between human perception and machine vision.

Armed with curiosity and a sense of wonder, our team embarked on a journey with CLIP, OpenAI's vision-language model that promised to bridge the gap between pixels and words. The mission sounded simple: find text descriptions that achieve the highest similarity scores with five given images. As we quickly discovered, CLIP doesn’t just see images, it interprets them through patterns, training data, and mathematical relationships, weighing every detail from tone to phrasing to how “human” a description sounds.

## Learning to Speak CLIP's Language

Our early experiments revealed CLIP's unique personality. Simple word choices often fell flat, while subtle phrasing changes made all the difference. We discovered that adding "a photo of" before nouns, including specific colors, and describing spatial relationships consistently boosted scores.

Abstract or emotional language rarely helped, CLIP preferred concrete, visual details. What began as technical testing quickly became a fascinating translation exercise between human intuition and AI pattern recognition. Each image became a puzzle where we had to think like the model to find the perfect caption key.

### The Sunset That Spoke in Color
Started with what we thought would be easy: a warm countryside sunset, a silhouetted tree, and birds flying across the orange sky. “Sunset,” we typed. Score: 0.2656.

Not bad… but not thrilling either. We tried “A photo of a sunset,” nudging the score slightly to 0.2788. Then we got ambitious:

“An image of an orange sunset with a silhouetted tree with a flock of birds.”

<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/718165fe-e231-4e8f-8d60-57c90bfadc32" />
</p>
<p align="center">
  <a href="https://images.pexels.com/photos/36744/agriculture-arable-clouds-countryside.jpg">Image Link</a>
</p>

Boom — 0.3608. Color, composition, and movement suddenly mattered. CLIP rewarded detail, and we were surprised.



### The Portrait That Rewarded Simplicity
Next came a calm black-and-white photo of a dog sitting against a white background. I began with “dog” (0.2827)—simple, direct, and surprisingly effective. We tried “puppy,” “hound,” and “pitbull,” thinking specificity might help, but the scores barely budged. Even “portrait” didn’t move the needle much.

Adding details like “black-and-white dog,” “studio portrait,” and “dog on white background” nudged the score up slightly, but not much. CLIP seemed happy with clarity over flourish.

Finally, the longer caption:


<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/0a1845cf-e750-4757-a675-978b30bf0cec" />
  <p align="center">
  <a href="https://images.pexels.com/photos/825947/pexels-photo-825947.jpeg">Image Link</a>
</p>

“An image of a studio portrait of a dog on a white background, high-key lighting.”

Score: 0.3486. Clear, structured captions win. Lesson learned.

### The Forest That Confused and Surprised Me
A foggy forest, trees fading into mist. I started with “mist” (0.2688) and tried “forest,” “fog,” and “woods,” but none surpassed it.

“A photo of a foggy…” (0.2957) — awkward, incomplete, but slightly better. CLIP doesn’t care about grammar; keywords matter more than elegance.


<p align="center">
  <img width="500" height="500" alt="Screenshot 2025-10-14 at 3 07 47 PM" src="https://github.com/user-attachments/assets/1fc5f1f8-b793-43f2-aefe-06c22088dc5b" />
  <p align="center">
  <a href="https://images.pexels.com/photos/34044163/pexels-photo-34044163.jpeg">Image Link</a>
</p>

Then the shocker:

“A photograph of a foggy forest with two unmade beds in autumn.”

Score: 0.3662. There were no beds! CLIP was rewarding semantic overlap in embeddings, not literal correctness. That’s when we truly grasped its quirks.


### The Puppy That Taught Me About Style
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

### The Room That Valued Realism
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

After uncovering CLIP's patterns with the five assignment images, we designed our own ultimate challenge: creating an image-caption pair from scratch that would achieve the highest possible similarity score. This was our chance to apply everything we have learned about how CLIP sees the world.

Rather than using existing imagery, we adopted a generative approach. We crafted a detailed scene description and used Gemini AI to bring it to life "a majestic stag standing in an abandoned library reclaimed by nature, with sunbeams filtering through broken windows.The mood is serene, melancholic, and awe-inspiring."

<p align="center">
  <img width="500" height="500" alt="" src="mygeneratedimage.png" />
  <br>
  <em>This image was generated by Gemini </em>
</p>

### The Search for Perfect Words

We tested 14 different captions, from simple descriptions like "a deer in a library" to poetic versions like "a stag lit by golden sunbeams in a library filled with books." Each caption represented a different approach to describing the same complex scene.

| Type                     | Example                                                        |
| ------------------------ | -------------------------------------------------------------- |
| *Minimalist*             | “a deer in a library”                                          |
| *Moderately descriptive* | “a stag in an old library with vines and bookshelves”          |
| *Highly detailed*        | “a stag lit by golden sunbeams in a library filled with books” |
| *Atmospheric*            | “a majestic stag inside a cathedral-like library”              |

The winner surprised us in its simplicity: "a stag standing in a sunlit, overgrown library" Score: 0.3451

This progression allowed us to examine how caption complexity affects CLIP’s embedding alignment and identify the balance point between descriptiveness and semantic precision.

CLIP revealed its preferences through this optimal pairing:

- Concrete beats abstract: "Sunlit" and "overgrown" outperformed "majestic" or "cathedral-like"
- Action matters: Including "standing" helped more than static descriptions
- Efficiency wins: Four clear elements worked better than complex phrasing
- Visual precision: Environment details ("overgrown library") proved crucial



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







