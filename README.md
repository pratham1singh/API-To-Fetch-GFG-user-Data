# GeeksforGeeks User Data API

This API allows you to fetch user data from GeeksforGeeks, including the number of problems solved, ranking, college name, monthly score, overall score, and names of problems solved category-wise.

## Getting Started

To fetch user data, make a GET request to the following endpoint:
https://gfg-api-fefa.onrender.com/USER_NAME

Sometimes due to network and traffic, this can take s to 2s time or some delay.
This is a completely free API with unlimited API calls.
## Advice
- As I have hosted this application on a free platform this may be slow in response.
- I advise you to clone this and host individually then use it if you want a quick response.
- Code Repo https://github.com/pratham1singh/GFG_API

## Response Format

The API response will be in JSON format and will include the following fields:

- `problems_solved`: Number of problems solved by the user
- `ranking`: User's ranking on GeeksforGeeks
- `college_name`: Name of the user's college
- `monthly_score`: User's monthly score
- `overall_score`: User's overall score
- `problems_solved_category_wise`: Names of problems solved by the user, categorized

## Sample Response

```json
{
   
    "instituteName": "Pranveer Singh Institute of Technology (PSIT) Kanpur",
    "languages": "Python, Java, C++",
    "rank": "174",
    "streak": "11",
    "overallScore": "620",
    "monthlyScore": "2",
    "totalSolved": "227",
    "easy": [
        "Problem 1",
        "Problem 2",
        ...
    ],
    "medium": [
        "Problem 1",
        "Problem 2",
        ...
    ],
    "hard": [
        "Problem 1",
        "Problem 2",
        ...
    ]
}
