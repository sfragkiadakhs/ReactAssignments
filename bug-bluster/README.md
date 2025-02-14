# Getting Started with bug-bluster

The purpose of this application is to understand the use of Reducers in React.

The application use-case is a ticketing-system.\
From top-to-bottom the following UI elements can be viewed:

- A form with fields title, description and priority, that allows the user to create or edit tickets.
- A list with the tickets that have been created so far, sorted by default from high-to-low priority(our available priorities are: low, medium or high).

Because our tickets have different states we use a ticket Reducer to manage these states.
Our states with their available actions incude:

- a state for our tickets with action.type {"ADD_TICKET","UPDATE_TICKET" and "DELETE_TICKET"},
- a state that corresponds to the existence of a current editing ticket with action.type{"SET_EDITING_TICKET" and "CLEAR_EDITING_TICKET"}
- and a state that stores how we want to sort our tickets when using action.type = "SET_SORTING".

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.
