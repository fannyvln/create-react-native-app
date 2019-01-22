```javascript
import * as Loadable from "react-loadable";
import { loaderComponent as Loading } from "./loader/loaderComponent";

const myLoadable = (opts) =>
    Loadable({
        delay: 600,
        loading: Loading,
        timeout: 5000, ...opts});

export const offerPage = myLoadable({
    loader: () => import("../containers/offer/offerContainer" /* webpackChunkName: "offer" */),
});

export const cartPage = myLoadable({
    loader: () => import("../containers/cart/cartPageContainer" /* webpackChunkName: "cart" */),
});
```
