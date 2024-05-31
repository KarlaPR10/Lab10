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
