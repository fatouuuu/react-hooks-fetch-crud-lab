# Steps to complete lab

In the QuestionList component:

    Use the useEffect hook to make a GET request to the API to fetch all questions when the component is first rendered.
    Add a new function, handleDelete, which will make a DELETE request to the API to delete a question. Use the fetch() function to make the request and make sure to pass the appropriate headers and body, as described in the prompt.
    Pass the handleDelete function as a prop to each QuestionItem component so it can be called when the user clicks the delete button.
    Add a new function, handleCorrectIndexChange, which will make a PATCH request to the API to update a question. Use the fetch() function to make the request and make sure to pass the appropriate headers and body, as described in the prompt.
    Pass the handleCorrectIndexChange function as a prop to each QuestionItem component so it can be called when the user changes the correct answer dropdown.
    Update the state variable "questions" when the user deletes a question or changes the correct answer dropdown.

In the QuestionForm component:

    Add a new function, handleSubmit, which will make a POST request to the API to create a new question. Use the fetch() function to make the request and make sure to pass the appropriate headers and body, as described in the prompt.
    Use the useEffect hook to make the formData state variable accessible in the handleSubmit function.
    Update the handleSubmit function to also update the questions state variable in the parent component (App) with the new question.

In the App component:

    Add a new state variable "questions" and use the useState hook to initialize it as an empty array.
    Pass the "questions" state variable as a prop to the QuestionList component so it can use it to render the question items.
    Update the questions state variable when a new question is added or a question is deleted or updated.
