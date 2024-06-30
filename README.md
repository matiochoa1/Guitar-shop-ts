# Guitar-shop-ts
In this project I developed a Guitar Shop with React + Tailwind CSS.

The project has been built with the following structure.
We have the main app.tsx and two components (Header and Guitars).
I've created a Custom Hook called useCart which makes usage of other hooks such as useState, useEffect and useMemo. Within the custom hook I've built most of the functions that are related to the cart, such as showing the guitars in the cart, increasing the quantity of an item inside the cart, decreasing it, removing it and clearing the cart + storing all the interactions of the user in localStorage. 
Then all of this functions are passed via props in the Header component which is the one that contains the cart.

Guitar component on the other hand is only in charge of displaying all the guitars in the UI. And its structure is very simple since it's only iterating over all the guitars in a GIST component and it's also making usage of the "addCart" function coming from our custom hook and later being passed via Props to the component itself to be used onClick.

This project was built to just work in the experience of creating a customHook but I'm going to build the same website but now making usage of useReducer.
