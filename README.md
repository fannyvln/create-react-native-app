```javascript
export const loadingComponent = (timedOut?: boolean) =>
    timedOut ?
        <p>Loading error, please try to refresh page</p>;
        : <CircularProgress size={80} thickness={3} variant="indeterminate" />

```
