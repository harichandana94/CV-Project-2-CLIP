# My CLIP-Challange

It all started with a simple challenge: could we find the perfect words that make an AI see an image the way we do?

Armed with coffee, curiosity, and five random images, our team set out to test CLIP, OpenAI’s vision-language model that claims to understand both pictures and text. The goal sounded simple enough — find the words or captions that get the highest similarity scores between image and text embeddings.

But as soon as we started, it became clear: CLIP has opinions. It doesn’t just look at an image and say, “Oh, that’s a cat.” It weighs every detail — tone, phrasing, and even how “human” your description sounds.

Our early attempts were rough. One word felt too vague, another too specific. Sometimes we nailed it, other times CLIP stubbornly disagreed. We weren’t just tuning a model; we were trying to speak its language.

## Where the Fun Began

It turns out, CLIP is picky — almost too picky. One wrong adjective and your score tanks. But tweak the phrasing just a little — add “a photo of,” change “dog” to “puppy,” or throw in a poetic twist — and suddenly CLIP believes you understand its language.

That’s when we realized: this wasn’t just a coding project. It was a game of translation, creativity, and a little bit of mind-reading between human and machine.

## The Portrait That Rewarded Simplicity
The next image was a calm black-and-white picture of a dog sitting against a white background, looking straight into the camera. I started off with the word “dog” (0.2827) pretty basic, but it actually worked better than I expected. Then I tried changing it to “puppy,” “hound,” and “pitbull,” thinking being specific might help, but the scores barely changed. Even “portrait” didn’t make much difference.

I thought maybe adding more detail would help, so I tried things like “black-and-white dog,” “studio portrait,” and “dog on white background.” The scores went up a little, but not much. It felt like CLIP was happy with simple and direct descriptions.

Finally, I tested a longer caption:

“An image of a studio portrait of a dog on a white background, high-key lighting.”

That one finally worked 0.3486, my best score for this image. I learned that CLIP actually prefers clear and straightforward captions.

## The Forest That Confused and Surprised Me
The third image looked like something out of a dream a foggy forest where the trees faded into the mist. I began with the word “mist” (0.2688), which felt right for the mood. Then I tried a few others like “forest,” “fog,” and “woods,” but none of them really beat that first choice.

When I moved to captions, “A photo of a foggy” (0.2957) sounded awkward but still got a slightly higher score, which was funny because it wasn’t even a complete phrase. It showed how literal CLIP can be sometimes it doesn’t care about grammar as long as the keywords match the image.

Then came the real surprise. The best caption turned out to be:

“A photograph of a foggy forest with two unmade beds in autumn.”

Even though there were obviously no beds in the picture, this caption scored the highest 0.3662. That’s when I realized CLIP doesn’t always focus on logical accuracy. It looks for visual and contextual overlap in the embeddings, even if the sentence doesn’t make sense.
