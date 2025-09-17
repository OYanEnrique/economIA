[Leia em português](README-ptbr.md) 

# 🤖 AIconomy: Your Personal Economics Guru

Tired of searching through endless, disorganized notes right before an exam? Frustrated with generic AI answers that have clearly never suffered through a Macroeconomics lecture?

**Fear not!** I present **AIconomy**, an AI agent that has been force-fed my actual university notes. This isn't just any AI; this is an AI with a degree in progress, specializing in surviving Economics 101.

## The Problem: Data Chaos vs. The Final Exam

Let's be real, our notes are a mess. They're a chaotic treasure trove of vital information, scribbled insights, and desperate pleas to the gods of economics. This is "unstructured data," and it's pure gold, but trying to find a specific concept in it is like trying to find a single, non-depressed student during finals week.

## The Solution: An AI That Does the Reading For You!

The **AIconomy** agent brilliantly solves this problem. By using a technique called Retrieval-Augmented Generation (RAG), it transforms that chaotic pile of `.txt` files into a searchable, intelligent knowledge base.

**How it helps you study:**
* **Precision Answers**: Ask a specific question like "What was the deal with Mercantilism?" and get an answer based *only* on what the professor taught (and what I managed to write down). No more weird, unrelated facts from the internet!
* **Concept Connection**: You can ask it to connect ideas across different subjects. "Create a debate between Adam Smith and Karl Marx" becomes a trivial task, not a 3-hour library session.
* **Instant Review**: It's the ultimate study buddy. It never gets tired, never tries to change the subject to last night's game, and is available 24/7.

## Technical Guts & Glory

* **The Brains (LLM)**: Powered by the lightning-fast Llama 3 via Groq. It thinks faster than you can say "supply and demand."
* **The Memory (Vector Store)**: Uses FAISS to create a high-speed, searchable vector database of my notes. It's like a photographic memory, but for economics.
* **The Librarian (LangChain)**: The framework that orchestrates the whole process, ensuring the right notes are retrieved to answer your questions.

## How to Power Up the Agent

1.  **Clone the Repo**: Get all the files onto your machine.
2.  **Upload to Colab**: Open the `AgenteIAEconomia.ipynb` notebook in Google Colab.
3.  **Feed the Machine**: Make sure to upload the `.txt` files with the notes (`Economia Política.txt`, `História econômica geral.txt`, `Macroeconomia.txt`) to the `/content/` directory in your Colab session.
4.  **Give it the Keys**: You'll need a free API key from [Groq](https://groq.com/). Save this key in your Colab "Secrets" with the name `GROQ_API_KEY`.
5.  **Run All Cells**: Sit back, run the notebook, and watch the magic happen.
6.  **Ask Away!**: Go to the last cell and type your most mind-bending economics questions in the `pergunta` variable.

### Example Session

```python
# What you do:
pergunta = "create a fight between karl marx and adam smith"

# What the AI does (based on my notes!):
--- Pergunta ---
create a fight between karl marx and adam smith

--- Resposta Gerada ---
Karl Marx: "Mr. Smith, your 'invisible hand' is just a pickpocket for the bourgeoisie, stealing the surplus value created by the proletariat!"

Adam Smith: "My dear Marx, you see exploitation everywhere! My 'invisible hand' is the harmony of self-interest creating societal good. Your system creates equal misery for all, except for those in charge of the 'equality'."
```
