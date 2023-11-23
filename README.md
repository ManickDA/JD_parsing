# JD_parsing


1. Utility Functions:
* A defined function to extract text between two specified characters using a regular expression.
* A defined function that Prepares the skill data from the job description text.
* A defined function that generates a response using the Google Palm Language Model.
* A defined function that extracts skills and experience from the job description using the Google
Palm Language Model.
2. Hybrid Similarity Function:
* A defined function that calculates the hybrid similarity between job description skills and resume
skills. It includes direct string matching, Levenshtein distance for partial matching, and checks if the
skill is present in the resume skills.
3. Job Description Example:
* when we Provide an example of a job description, calls the function that is defined to extract skills
and experience from it.
4. Matching Process:
* Apply the defined hybrid_similarity function to each resume in the dataset and stores the results in
a DataFrame (final_data).
* Calculates an experience tag (1 if resume experience is greater than or equal to JD experience, 0
otherwise).
* Computes a matching score based on skill similarity and experience tag.
* Sorts the results by the matching score in descending order.
5.Top Matches:
Extracts the top 5 matches and removes unnecessary columns.
6.The models or techniques used in the code include:
* Google Palm Language Model for natural language generation.
* Fuzzy string matching using the fuzzywuzzy library.
* Hybrid similarity calculation using a combination of direct string matching, Levenshtein distance,
and set operations.
* DataFrame operations and sorting using pandas
