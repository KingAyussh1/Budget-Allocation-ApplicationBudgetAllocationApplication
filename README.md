# Budget-Allocation-ApplicationBudgetAllocationApplication

It has the following six components:-Budget, ExpenseItem, ExpenseList, ExpenseTotal (Spent so far), Remaining, AllocationForm. All of these components will be using redux for state management through AppContext.js.

In AppContext.js:-I have created a reducer, which is used to update the state, based on the action. Then I will set the initial state for the departments. I have created the Provider component which wraps the components I want to give access to the state. Here, I have added an initial budget, creating a Provider component, setting up the useReducer hook which will hold my state, and allow me to update the state via dispatch.

Details of the six components:-

In Budget.js-I will be adding text and value for my budget. I will be importing app context and the useContext hook, and pass my AppContext to it - this is how a component connects to the context in order to get values from global state.
In Remaining.js-I will be importing expense and budget from context and getting the remaining value using subtraction.
In ExpenseTotal.js-I will be adding useContext and AppContext. Taking the expenses from state.
In ExpenseList.js-I will be using the map function to display the Expenseitem component.
In Expenseitem.js-I will be importing dispatch from Context, which allows you to dispatch a delete action, creating a function that gets called when the delete icon is clicked.
In AllocationForm.js-I will be creating an expense object, containing the name and the cost. This is what will get dispatched as the payload, and what I will use to update the state.
