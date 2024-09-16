# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?
Context API helps solve the problem of of easily passing props down to many layers of components, without prop drilling or setting up redux. 

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
actions are objects that are dispatched to the reducer, which will then determine which case statement is exectued and with what information (payload from the action). The store is the single source of truth in redux becasue you are setting up your state and reducers all in one place (store) to then be used (provided) accross your applicaiton.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?
redux thunk allows us to use asynchronous functions as actions. without thunk this would attempt to pass the entire function to the reducer, which would obviosuly cause an error. Thunk will look at what is being returned from your action. If it is an object, then treat it normally. If it is a function, then go ahead and exectute that function, which will also automatically receive dispatch as an argument passed into it (to be used within the function)

4. What is your favorite state management system you've learned and this sprint? Please explain why!
Redux 110%. I enjoy redux the most because it feels neater and more organized, you have access to redux dev tools, and you have access to middleware.