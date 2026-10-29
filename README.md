# Cook recipe generator (RAG)

Ratatouille LLM is a recipe assistant built with CrewAI, OpenAI, and Serper web search. Four sequential agents research recipes, filter dietary restrictions, rank candidates, and format the top three recipes.

## Files

- `ratatouille_llmfinalproject.py`: original, unchanged Colab export. It contains notebook syntax and is not a standalone Python script.
- `Cook_recipe_generator_RAG.ipynb`: notebook reconstructed from the export. The Colab secrets import is moved before its first use, and installation uses `%pip`.
- `requirements.txt`: dependencies without version pins; the original export specifies no versions.

## Run in Google Colab

1. Upload and open `Cook_recipe_generator_RAG.ipynb` in Google Colab.
2. Add `OPENAI_API_KEY` and `SERPER_API_KEY` in Colab Secrets and enable notebook access.
3. Edit `topic`, `dislikes`, `allergies`, and `preferences` in the code cell.
4. Run the cell. Requests use external APIs and may incur charges.

The current example uses tuna, excludes bread and lettuce, and requests no oil. The workflow retrieves web search results; the supplied code does not implement a vector database or document indexing pipeline.

Recipe generation has not been executed or validated here. Check ingredients independently when allergies are involved.
