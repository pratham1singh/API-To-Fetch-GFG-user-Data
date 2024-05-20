<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GeeksforGeeks User Data API</title>
</head>
<body>
    <h1>GeeksforGeeks User Data API</h1>
    <p>This API allows you to fetch user data from GeeksforGeeks, including the number of problems solved, ranking, college name, monthly score, overall score, and names of problems solved category-wise.</p>

    <h2>Endpoint</h2>
    <p>To fetch user data, make a GET request to the following endpoint:</p>
    <pre><code>https://gfg-api-3.onrender.com/USER_NAME</code></pre>
    <p>Replace <code>USER_NAME</code> with the actual username of the GeeksforGeeks user whose data you want to fetch.</p>

    <h2>Response Time</h2>
    <p>The API may take between 1 to 2 seconds to fetch and return the data.</p>

    <h2>Example</h2>
    <p>To fetch data for a user with the username <code>john_doe</code>, you would make a GET request to:</p>
    <pre><code>https://gfg-api-3.onrender.com/john_doe</code></pre>

    <h2>Response Format</h2>
    <p>The API response will be in JSON format and will include the following fields:</p>
    <ul>
        <li><code>problems_solved</code>: Number of problems solved by the user</li>
        <li><code>ranking</code>: User's ranking on GeeksforGeeks</li>
        <li><code>college_name</code>: Name of the user's college</li>
        <li><code>monthly_score</code>: User's monthly score</li>
        <li><code>overall_score</code>: User's overall score</li>
        <li><code>problems_solved_category_wise</code>: Names of problems solved by the user, categorized</li>
    </ul>

    <h2>Sample Response</h2>
    <pre><code>
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
    </code></pre>

    <h2>Notes</h2>
    <ul>
        <li>The API is read-only and does not require authentication.</li>
        <li>Ensure you handle the response time in your application to avoid timeouts.</li>
    </ul>
</body>
</html>
