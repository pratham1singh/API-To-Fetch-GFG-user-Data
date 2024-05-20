# GeeksforGeeks User Data API

This API allows you to fetch user data from GeeksforGeeks, including the number of problems solved, ranking, college name, monthly score, overall score, and names of problems solved category-wise.

## Getting Started

To fetch user data, make a GET request to the following endpoint:
https://gfg-api-3.onrender.com/USER_NAME

Sometimes due to network and traffic, this can take s to 2s time or some delay.
This is completely free API with unlimited API calls.

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
    "problems_solved": 150,
    "ranking": 345,
    "college_name": "ABC University",
    "monthly_score": 1200,
    "overall_score": 5000,
    "problems_solved_category_wise": {
        "Easy": ["Problem 1", "Problem 2"],
        "Medium": ["Problem 3", "Problem 4"],
        "Hard": ["Problem 5"]
    }
}
