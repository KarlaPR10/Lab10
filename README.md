Task 1: Analyze each code snippet to identify potential performance issues. Look for common problems such as:
  Inefficient loops that can be optimized or rewritten.
  Redundant computations that can be simplified or eliminated.
  Excessive memory usage due to poor data structure choices.
  Unoptimized database queries that slow down data retrieval.
Task 2: Document your initial findings for each snippet, noting what you believe are the key areas for improvement.
  Implementing Optimizations:
Task 3: Refactor the code based on your analysis. Apply optimization techniques such as:
  Streamlining loops to reduce computational overhead.
  Implementing effective caching mechanisms where appropriate.
  Reducing complexity by improving conditional logic or function calls.
  Optimizing data structures for better memory management.
  Enhancing database queries to reduce load times.
Task 4: Ensure that each optimization is documented. For every change you make, write a brief explanation of:
  What the specific issue was.
  How you addressed it with your optimization.
  Why you chose that particular approach.
  Evaluation:
Task 5: Compile a report summarizing the optimizations you implemented. The report should include:
  A description of the original code problems.
  Detailed explanations of the changes made.
  Discussion on the expected or observed outcomes of these changes in terms of performance improvement.

    Deliverables:
    A completed set of optimized code snippets.
    A written report detailing the changes made, the reasoning behind each decision, and any observations or expected outcomes related to performance improvements.

    Provided Code Snippets:
      JavaScript Snippet

  <img width="585" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/d8c260e1-f93f-4871-a9cc-bc1c83e93c81">

      
    The provided code is inefficient due to the excessive DOM manipulation and loop handling. Here’s a breakdown of the issues:
    
    Excessive DOM manipulation: The code creates a new li element for each item in the items array and appends it to the list element. This can lead to a significant number of DOM mutations, which can be slow and inefficient.
    Inefficient loop handling: The loop iterates over the items array, creating a new li element for each item. This can be optimized by using a more efficient loop handling approach.
    To optimize the code, we can use the following approach:
    
    Improved Code

<img width="600" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/bc5ae92b-3321-4d47-9790-105bd76f7276">



    Here’s what’s changed:
    
    Use map() and join(): Instead of creating a new li element for each item and appending it to the list element, we use the map() method to create an array of HTML strings for each item. We then use the join() method to concatenate these strings into a single string.
    Set innerHTML directly: We set the innerHTML property of the list element directly with the optimized HTML string. This eliminates the need for excessive DOM manipulation.
    By using this optimized approach, we can significantly improve the performance of the code.

  <img width="729" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/d93add80-b7f2-49d6-aea4-233a938e3f52">

  The provided code snippet is a basic implementation of a LoadProducts method that retrieves products from a database using their IDs. To optimize this method, we can consider the following suggestions:

    Use a more efficient database query: Instead of making 100 separate database queries to retrieve products by ID, we can use a single query to retrieve all products at once. This can be achieved by using a SELECT statement with a WHERE clause that filters products by ID.
    Use a more efficient data structure: The current implementation uses an ArrayList to store products, which can be slow for large datasets. We can consider using a more efficient data structure such as a HashSet or a HashMap to store products.
 <img width="842" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/16f2ddf7-7099-40ac-bb3a-b8c3c88b884a">
          
    Avoid unnecessary database calls: The current implementation retrieves all products from the database, even if the user only needs a subset of products. We can consider adding a parameter to the LoadProducts method that allows the user to specify the range of IDs they need.
    Here’s an updated implementation that incorporates these suggestions



<img width="550" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/ad45dd0d-2039-4c9e-b48d-5b820298fe30">

    The provided code can be optimized by using a single loop and avoiding the creation of a new list for each iteration. Here’s the optimized code:

  <img width="403" alt="image" src="https://github.com/KarlaPR10/Lab10/assets/138635602/c0ea1808-ad87-4ef8-8287-6ef22216364d">


    
    Explanation
    
    The original code uses a foreach loop to iterate over the input list data and adds each element to the result list result after performing some operation. The operation is either multiplying the element by 2 if it’s even or by 3 if it’s odd.
    
    The optimized code achieves the same result using a single loop and a conditional expression in the add method. The conditional expression d % 2 == 0 ? d * 2 : d * 3 checks whether the element is even or odd and performs the corresponding multiplication. This eliminates the need to create a new list for each iteration and reduces the number of operations.





