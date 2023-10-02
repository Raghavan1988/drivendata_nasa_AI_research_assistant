# drivendata_nasa_AI_research_assistant

## Steps to run the terminal program, ## Risk: Hallucination by LLM is the main challenge
1. Get an OPEN AI API KEY
2. Download the following files from S3
   - Annoy Index for (Arxiv articles upto 12/2022)
   - Annoy Index for (Arxiv articles since 12/2022 to 08/2023)
   - Arxiv data with metadata json file (upto 12/2022)
   - Arxiv data with metadata json file (since 12/2022 to 08/2023)
  


3. pip install -r requirements.txt
4. python task_identify_research_gaps.py
 
![Urban planning research gaps and opportunities](https://github.com/Raghavan1988/drivendata_nasa_AI_research_assistant/assets/493090/b421982a-6498-45de-9477-799bebabb031)

example: 
input field query: urban planning
- solution retrieved top articles from annoy index
- summarized and identified research gaps
- identified *Artificial Intelligence* as orthogonal field to draw inspirations.
- Cross pollinated and recommended ideas based on Artificial Intelligence field to *Urban Planning*

5. python task_identify_leading_experts.py
   ![leading experts](https://github.com/Raghavan1988/drivendata_nasa_AI_research_assistant/assets/493090/66d39951-2f70-4c60-aca6-dd8cffadf235)
   example query: deep learning in earthquakes and volcanoes
- solution retrieved top articles from annoy indexy
- Solution analyzed authors, identifed who collaborated with who and recommends authors based on what they published.
   The solution shows [Arnaud Mignan](https://www.google.com/search?channel=fs&client=ubuntu-sn&q=Arnaud+Mignan+site%3Aarxiv.org) and a [sample ARXIV article (2019)](https://arxiv.org/abs/1910.01178)



7. task_identify_related_conceps.py
   - Solution takes in input field and the personal field of the user.
   - Analyzed top articles from the input field and generated concepts
   - When the user's field is different, it outputed analogy to help with understanding.
  
      blackhole: For me who has a background in Machine Learning, the solution provided an analogy of a bottleneck layer in Neural networks where information gets compressed.

![related conceps](https://github.com/Raghavan1988/drivendata_nasa_AI_research_assistant/assets/493090/048103be-db6f-48ad-973d-95d4bc58f406)
