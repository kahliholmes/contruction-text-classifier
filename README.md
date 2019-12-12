# Construction Text Classifier (Hackathon Project)

This project was a product of the 2019 Procore Hackathon. Completely educational and exploratory, but there are use cases for Procore.

If we can start identifying what people are talking about within procore, we can start creating connecitons amongst other vendors based on specialty, identify and leverage potential puchase intents based on subject, or simply provide more insights to GCs on their projects (ex: 85% of project delays/rfi's were linked to Concrete and Masonry work)

Unfortunately I was unable to get good training data for this experiement (turns out our db is filled with test/demo/orientation/foobar dummy accounts that mucked up the data pool a lot). You'll notice most of what I did was from data I accumulated by hand (don't laugh too hard at it, I tried). Most of the text I'll be handling in this process will be common questions brought up from RFIs and Submittals

Two approaches were done
- a Neural network bag-of-words approach that handled stemming words down to baseline tokens (acheived better results)
- a CNN built with Keras that leveraged [GloVe](https://nlp.stanford.edu/projects/glove/) (pretrained vectorized word representations) for word embedding

Note: You will have to download GloVe.6B.zip and reference the glove.6B.100d.txt file in order to get the later project to run
