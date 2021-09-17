## 1. Install Dependencies

```
npm install react-router-dom
```

## 2. Initialize and wrap Provider

```jsx
import { BrowerRouter } from "react-router-dom";

ReactDOM.render(
  <BrowserRouter>
    <App />
  </BrowserRouter>,
  document.getElementById("root")
);
```

## 3. Routes

```jsx
import { Route } from "react-router-dom";

function App() {
  return (
    <div>
      <Route path="/welcome">
        <h1>Welcome</h1>
      </Route>
      <Route path="/products">
        <h1>Products</h1>
      </Route>
    </div>
  );
}
```

## 4. Links and Navlinks

```jsx
import { Link, NavLink } from "react-router-dom";

function App() {
  return (
    <div>
      <NavLink activeClassName="active" to="/welcome">
        Go to welcome page
      </NavLink>
      <NavLink activeClassName="active" to="/products">
        Go to products page
      </NavLink>
      <Link to="/cart">Go to Cart</Link>
    </div>
  );
}
```
