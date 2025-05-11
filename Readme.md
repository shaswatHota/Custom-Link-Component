# CLink (Custom React NavLink Component)

A lightweight and highly customizable React component that replicates the behavior of `react-router-dom`'s `<NavLink>`, but uses a `<div>` element instead of an `<a>` tag. Useful when you need advanced styling or interaction control without HTML anchor limitations — especially when using Tailwind CSS.

## ✨ Features

- Uses a `<div>` instead of `<a>` for full styling freedom
- Supports conditional styling via `isActive` state
- Fully integrates with `react-router-dom` for routing
- Simple API similar to React Router's `<NavLink>`

## 🚀 Usage

```jsx
import CLink from './components/CLink'; // or wherever the file is located

<CLink
  to="/home" //to the route to want to go when clicked
  className={({ isActive }) =>
    `mb-2 pl-5 block hover:bg-[#e1e3e6] ${isActive ? "bg-[#e1e3e6]" : ""}` //what do you want to do when the route is active
  }
>
  Home 
</CLink>
