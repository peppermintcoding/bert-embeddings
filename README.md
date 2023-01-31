# bert-embeddings
Playing around with Bert Tokenizer

Goal of this experiment is to generate a meaningful color for every word.

### Reduce Embedding Space

The Bert embeddings and others create vectors in a high dimensional space.
To reduce that complexity and to get to the normal 3D space used for colors
either as (RGB or others) we need to use `PCA`.

For this we need already computed embeddings to feed it into the `PCA`
algorithm and get embeddings for new words or sentences.

This can either mean the colors change the more word are fed in after
one another or it can mean, we precompute the space beforehand
with 100k or so most used words. With phrases this would be impractical.
