# anki-sentence-gen
A generator for sentence flashcards in Anki

# Motivation
From MoeWay's Sentence deck, the best way to build a solid base before immersion is through sentence flashcards. This allows you to understand the word in context as well as build a base for grammatical elements before you actually learn about grammar.

A challenge of this task will be to not introduce too many words that have not been learned yet (i+1 principle).

# Done Tasks

- Tester code that can autogenerate anki cards
- Sources for word frequency data
    - (Static, not updating) Hermit words data source that contains the most used words in every language
        - Caveat 1: This contains raw data like numbers, parentheses, etc. Needs to be cleaned.
        - Caveat 2: In languages like Chinese, Japanese, we are supplied with "base" words (single characters), but these can mean (and be pronounced in different  ways) depending on the context.
    - There are higher quality sources, to be constructed? e.g. a builder  that can construct phrases based on a sense of "difficulty"
- Local Ollama LLM  generation with laptop GPU. It appears this is slow.
    - Two routes:
        1. As HW improves, what direction will we take local LLM generation?
        2. Or, how could we outsource compute to the cloud?

# Features Roadmap

Anki format supports furigana for Japanese, so pinyin should be acceptable in Chinese too. At base level, we can simply define the words one-by-one after.

The MoeWay's deck also includes a native reader on the sentence. For an MP4. A further downstream project would be to generate  these automatically.
