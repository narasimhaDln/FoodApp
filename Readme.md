//function component syntax like this writing from scratch
// function App() {
// return <h1>welcome to javascript</h1>;
// }
// //another way to writing this
// Note:make sure to while writing react code in components write the starting letter is capital other wise we wil get error some files

//in this heading component i need call the inside the heading component i will calling the app component

/////component composition
// const Heading = () => (
// <div>
// <App />
// <h1>hello my name is</h1>
// </div>
// );

// javascript in side html code
//react element
// let title=<span>This is span tag</span>
// let arr = [1, 2, 3, 4, 56];
//react component
// const Heading = () => (
// <div>
// <App />
// {title}
// <h1>hello my name is</h1>
// <h2>{arr}</h2>
// <h3>{"My name is React" }</h3>
// </div>
// );
// const root = ReactDOM.createRoot(document.getElementById("root"));
// root.render(<Heading />);///<Heading></Heading> or </Heading> or {Heading()} 3 are same

//making the app level layout
//props are used to this are normal function properties ,,,it will give you object
{/_ //in our json data id not have means use index other wisw use unique in what evern given in your inside data ide like this key={Object.id} _/}
{resObj.map((res, index) => (
<RestaurantCard key={index} resObj={res} />
))}

Export/import;
Export two types:1.Default export
ex:export default componentName or variable name->which file ur created new file
import componentName from "./componentName/Header.js"->where you want
2.Named export;
ex: export const CDN_Link="link"
import {CDN_links} from "../utils/constants" ,file path

React hook -it is normal javascript function;
Main vary important hooks;
1.useState();
2.useEffect()
//creating state variable;
const [listOfRestaurants,setList]=useState([]);
or
const [listOfRestaurants,setList]=arr->this means array destructuring
first argument in array is current value;
2 argument in array is function update;
//Normal variable;
const listOfRestaurants=[]
###when ever our state variable is updated our react UI automatically rerender the UI in browser;

**\***Why react it so popular?
1.it is virtual dom
2.efficient dom manipulation;
3.react is render the vary fast;
4.find the difference between the virtual DOM and actual DOM it will update the UI fast way And automatically update the our UI

->when ever state variable change react is rerender the component
->we are working with input forms make sure to give callBack function for trigger (reconciliation cycle )the something and getting the what we trying to typing in input section:
Ex;
const [text,setText]=useState(")

<!-- <input onChange={(e)=>setText(e.target.value)}/> -->

<!-- features -->

Features:

Dynamic Data Handling: Uses useState to manage the list of food items and the app's state.
Data Fetching: Utilizes useEffect to fetch data when the component mounts or when specific state variables change.
Interactive UI: Users can interact with the food list, and the UI will update accordingly.
Responsive Design: The app is styled with CSS to ensure it looks good on different screen sizes.
Technologies Used:

React (with Hooks: useState, useEffect)
CSS for styling the user interface

Installation
To run this project locally:

Clone the repository:

bash
Copy code
git clone <repository-url>
Navigate into the project directory:

bash
Copy code
cd <project-directory>
Install the necessary dependencies:

bash
Copy code
npm install
Start the development server:

bash
Copy code
npm start

Usage
Once the app is running, you will see a list of food items. The app uses React's useState to manage the state of the food list and useEffect to fetch data from an API when the component is mounted.

Key Features of the App:

The food list is displayed dynamically based on the state.
The app fetches data from an external API using useEffect when the component is mounted.
The UI updates automatically when the state changes.
