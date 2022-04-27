# Angular Task

The app called Shopping cart app is a reactive app, where all components automatically react to new data.
For a  better user experience actions are immediately reflected in all components before data is uploaded to the server.
Angular services and reactive GUI elements are used for that purpose.

---

## Your Task

Your task is to fix a few issues with data synchronization across the app and to add few customization features.

### 1. Cart status is not shown until the user makes a change
- Make changes to cart service so that subscribing to changes immediately updates the state.
- Resubscribing to cart state should broadcast the most recent cart state, so that when component subscribes after events were broadcast, it still gets most recent state.

### 2. Cart item control has a potential memory leak
- Subscriptions in cart control component are left behind.
- Make sure components unsubscribe when they get destroyed. (You can also use async pipe)

### 3. Dynamic product template
- `ProductsList` component detects templates with `forProduct` directives to provide custom item template
- If product doesn't have 'type' property matching 'ofType' param it defaults to `default` template
- Modify `ProductsList` component so that when a custom template for `forProduct=let product ofType 'default'` is provided in **Content** (content-projected), it overrides built-in 'default' template.

---

For comprehensive feedback regarding the quality of your solution it is strongly suggested that you upload your code to the Devskiller.com online code editor.

## Setup

1. `npm install` to get dependencies
2. Start app with `npm run start` and point browser to `http://localhost:4200/`
3. Use `npm run test:watch` to see tests failing
4. Fix issues so that tests pass
5. Solve all issues mentioned here
6. Submit your code on DevSkiller platform to see if task is completed

## Good Luck!
