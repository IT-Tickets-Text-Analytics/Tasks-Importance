# Tasks-Importance
The task importance aspect reflects the level of attention that should be paid to certain task elements. We differentiate between the following levels of attention: standard (meaning common daily work), elevated (task performer should be cautious with certain task elements), and high (the process worker should be especially cautious with certain task elements). For extraction purpose, we propose a specific approach of Business Sentiment (BS). BS represents an emotional component of a task and its contextual importance perceived by a task performer. This latent information is extracted from task textual description with a BS lexicon and formalized using the mentioned qualitative scale of standard, elevated, and high. 

This repository contains the following files: Business Sentiment (BS) Lexicon, python file for identifying importance (BS) (as an input for python file serve tasks textual descriptions and BS Lexicon), excel file with the motivating example, threshold rules, and illustrative BS Lexicon (as an input for excel file serve threshold rules).

Below, we describe the main stages of Step 3. Importance Aspect Extraction.

Python code:(Importance_Extraction.py)
STAGE 1. BS lexicon reading and stemming
STAGE 2. Tasks corpus (2.1.) reading, special preprocessing
       (2.2.) keeping special symbols and uppercase and
       (2.3.) English language filtering
STAGE 3. Find words in the task text that match (3.1.) the BS lexicon expressions and (3.2.) the BS lexicon keywords. Count number of matched words and their total score
STAGE 4. Writing of matched words, their number and total score in the *.csv file

Excel *.csv file computing:(Importance_Calculation.xlsx)
STAGE 5. Calculation the normalized total score for each task text
STAGE 6. Importance identification
