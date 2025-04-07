# **LyricWeaver: Emotionally Resonant Song Lyrics Generation Using Transformer Synergy**

## Abstract

**LyricWeaver** represents an innovative leap in automated song lyrics generation, blending the generative prowess of a decoder-based transformer model, GPT-2, with the emotional and contextual finesse of a masked language model (MLM), RoBERTa. By training GPT-2 on an extensive corpus of song lyrics to produce coherent, artist-specific outputs and RoBERTa on poetry to imbue emotional depth, this project aims to craft lyrics that resonate both structurally and emotionally. Currently, the system generates lyrics by taking the name of an artist as input, enabling it to emulate distinct stylistic signatures while striving for artistic richness. This dual-model approach seeks to redefine the boundaries of AI-driven creativity, offering a tool that could inspire songwriters, enhance music production, and captivate audiences.

## Introduction

Song lyrics are more than words—they are vessels of emotion, rhythm, and identity, weaving stories that connect with listeners on a visceral level. The rise of artificial intelligence has opened doors to automating this creative process, yet many existing systems fall short in capturing the soul of music. Enter **LyricWeaver**, a project designed to merge the fluency of GPT-2 with the poetic sensitivity of RoBERTa, creating lyrics that are not only structurally sound but also emotionally evocative. At present, lyrics generation begins by providing the name of an artist, allowing the system to tailor its output to reflect specific musical styles. This initiative explores the synergy of transformer architectures, aiming to produce lyrics with the depth and artistry of human composition, with applications ranging from entertainment to creative collaboration.

## Motivation

The inception of **LyricWeaver** stems from a desire to fuse technology with the timeless art of music. Current lyrics generation tools often excel at mimicking style but struggle to convey the emotional weight that defines great songs. By integrating GPT-2, trained on song lyrics, with RoBERTa, fine-tuned on emotionally rich poems, we seek to fill this gap. The ability to generate lyrics based on an artist’s name adds a personalized dimension, making the tool adaptable for diverse creative needs. Beyond technical innovation, this project is fueled by a passion for music and a curiosity about AI’s potential to augment human expression. Its outcomes could assist songwriters facing writer’s block, provide fresh material for the music industry, or even serve as a therapeutic outlet through personalized lyric creation.

## Dataset Gathering

The backbone of **LyricWeaver** is a meticulously curated dataset of song lyrics and poems. Song lyrics were gathered through web scraping from platforms like Genius and other music databases, spanning genres from pop to hip-hop to folk. Poems, selected for their emotional and thematic richness, were sourced from public domain collections, literary archives, and online poetry repositories. To bolster this, we integrated datasets from Kaggle, amassing over 100,000 song lyrics and 50,000 poems. Preprocessing steps included removing special characters, standardizing text to lowercase, and tokenizing with the GPT-2 tokenizer for model compatibility. The dataset is organized to link lyrics with artist names, enabling the system to generate artist-specific outputs effectively.

## Experiments List

The development of **LyricWeaver** involves a comprehensive experimental roadmap:

1. **GPT-2 Training:** Fine-tune GPT-2 on song lyrics to generate fluent, artist-specific lyrics using artist names as prompts.
2. **RoBERTa Training:** Train RoBERTa on poems via masked language modeling to enhance emotional and contextual understanding.
3. **Model Integration:** Merge GPT-2’s generative capabilities with RoBERTa’s depth for emotionally resonant lyrics.
4. **Hyperparameter Optimization:** Adjust model architectures, learning rates, and batch sizes for peak performance.
5. **Line Addition:** Develop methods to append new lines, improving song structure and coherence.
6. **Phonetics Integration:** Incorporate phonetic analysis to align lyrics with musical rhythms.
7. **Alternative Models:** Test models like T5 or BART to benchmark against our current approach.
8. **Evaluation Framework:** Create metrics and human-involved methods to assess lyric quality.
9. **Context Expansion:** Address GPT-2’s context length constraints for longer, cohesive outputs.

## Experiments Conducted Till Now

Our progress to date includes foundational training for both models:

- **GPT-2 Training:** We trained GPT-2 on our song lyrics dataset with a batch size of 8, a learning rate of 5e-5, and 10 epochs. The model now generates coherent lyrics reflecting artist-specific styles when provided with an artist’s name as input. Initial outputs show fluency and stylistic alignment, laying a strong base for further refinement.
- **RoBERTa Training:** RoBERTa was trained on the poetry dataset using masked language modeling, with a batch size of 16, a learning rate of 2e-5, and 5 epochs. It excels at predicting masked words while preserving the emotional tone and metaphorical nuance of the poems, enriching the system’s contextual capabilities.

## Experiments Planned

Looking ahead, we aim to advance **LyricWeaver** with these experiments:

- **Model Integration:** Devise a strategy to blend GPT-2’s outputs with RoBERTa’s insights, balancing coherence and emotional impact.
- **Line Addition:** Implement algorithms to extend generated lyrics with new lines, addressing the current lack of structural completeness.
- **Phonetics Integration:** Use tools like the CMU Pronouncing Dictionary to add phonetic alignment, enhancing musicality.
- **Model Exploration:** Experiment with transformers like T5 or BART to identify potential improvements.
- **Multilingual Expansion:** Incorporate non-English datasets to broaden the system’s linguistic scope.
- **Context Length Solutions:** Tackle GPT-2’s token limitation through techniques like hierarchical generation or memory networks.

## Challenges

The journey of **LyricWeaver** has surfaced several hurdles:

- **Evaluation Metrics:** Measuring lyric quality is complex—standard metrics like BLEU miss emotional and artistic value. We’re developing a mixed approach with perplexity, sentiment analysis, and human feedback.
- **Model Integration:** Combining GPT-2 and RoBERTa seamlessly while retaining their strengths is technically challenging and under active exploration.
- **Phonetic Alignment:** Adding phonetic features for rhythm compatibility increases complexity, requiring specialized tools and knowledge.
- **Resource Scaling:** Larger datasets or multilingual expansion demand significant computational power, necessitating optimization.
- **GPT-2 Context Length Limitation:** GPT-2’s maximum context length is 1024 tokens, but we’re currently limited to 128 tokens in our implementation. This restricts the model’s ability to maintain coherence over longer lyrics, a critical issue we plan to address with innovative techniques.

## Conclusion

**LyricWeaver** stands as a bold step toward AI-powered lyrics generation, uniting GPT-2’s fluency with RoBERTa’s emotional depth to craft lyrics that sing with meaning. Currently, the system generates artist-specific lyrics by taking an artist’s name as input, with early results showing promise in style and coherence. As a mid-evaluation milestone, we’ve laid a solid foundation with trained models and a clear path forward—integrating the models, enhancing structure, and tackling challenges like GPT-2’s context length limit. The potential to revolutionize music creation, inspire artists, and explore AI’s creative frontiers drives us onward. Future efforts will refine our approach, expand dataset diversity, and overcome technical barriers, positioning **LyricWeaver** as a harmony of technology and artistry.

---


AI models can be found here:

https://drive.google.com/drive/folders/1bVGu2z9EQ7DyZzkgNSNYMfhdEtgm-ks4?usp=sharing
