##My CLIP-Challange##

When I first heard that CLIP could “understand” both images and text, I was amazed. A model that looks at a photo of a cat and instantly links it to the word cat? That sounded almost magical — until I tried it myself.

Very quickly, I realized something fascinating: CLIP isn’t perfect. It can be convinced, confused, or even tricked. The more I experimented, the more it felt like playing a strange game — me on one side, the model on the other — both trying to agree on what a picture means.

This project became less about getting the “right” answer and more about exploring the modality gap — the invisible space between how a machine reads an image and how it interprets words. Through trial and error, I learned how phrasing, structure, and even a single adjective can make CLIP “believe” an image matches a caption better than before.

In this post, I’ll walk through my experiments, show what worked (and what didn’t), and share how I tried to trick CLIP into higher scores — one caption at a time.

This project explores how Vision-Language Models, specifically OpenAI’s CLIP, connect images and text in the same feature space.
The goal was to understand how well CLIP matches an image with the right description and to explore what kinds of captions give the strongest similarity scores.

The challenge had two parts. In the first part, I tested CLIP on five given images to find the most accurate matching words and captions. In the second part, I used my own chosen images to see how far I could push the model to find captions with very high cosine similarity.
