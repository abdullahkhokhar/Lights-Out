This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

![](https://media.giphy.com/media/h8a4IWLhE3BmO7jKm7/giphy.gif)

## Component Design

### `App`

As often, this is a very simple component. It just renders the Board component.

### `Board`
The most sophisticated component. It will hold the state that represents the in-memory grid of true/false for lights-on/off. Since the state for the board lives here, this is also were the setState() calls will need to go — and therefore, all the functions that call setState().

### `Cell`
A simpler component. This will simply render a div, where the CSS classes will indicate whether this cell is lit or unlit. This is what the user clicks on — but it will need to call a function it receives from the Board, since that will need to update the state.
