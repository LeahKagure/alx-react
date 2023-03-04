0. **Write mapStateToProps** - Reuse the latest dashboard project you worked on in the React course `0x09-React_Redux_reducer` and install `react-redux`
1. **Create a small store** - In the `index.js` file, Create a store using `createStore` from Redux that would contain the `uiReducer` state. Implement a provider passing the store that you created to the main `App`
2. **Test MapStateToProps** - Export the `mapStateToProps` function you created if you haven't already, and in the `App.test.js` file, create a new suite to test the function and create a test that verify that the function returns the right object when passing the function
3. **Update mapStateToProps** - In the `App.js` file, update the `mapStateToProps` function to also pass to the component the value for `displayDrawer`. It should be connected to the Reducer attribute `isNotificationDrawerVisible`. Update the render function to the component to use the value `displayDrawer` coming from the props instead of the state
4. **Connect your actions creators** - In the `App.js` file, connect to the component the actions creators `displayNotificationDrawer` and `hideNotificationDrawer`. You should use the simplified version for the `mapDispatchToProps`. No need to import `bindActionCreators`. Modify the render function of the component to use the functions passed within the props instead of the action within the Class component
5. **Refractor your code** - In the `App.js` file, you can delete the old function `handleDisplayDrawer`, `handleHideDrawer`, remove any state property related to the display of the drawer and any binding in the constructor
6. **Update your tests** - You can now refractor the `App.test.js` file
7. **Async actions & Thunk middleware** - Implement the `LoginRequest`/`logout` actions creators across the entire application. `LoginRequest` is calling an API and is Async.
8. **Connect LoginRequest to the App** - Modify the file `App/App.js`
9. **Connect user state to the Footer** - Modify the file `Footer/Footer.j`
10. **Connect Logout action creator to the Header** - Modify the file `Header/Header.js`
11. **Modify the uiReducer** - With the entire login request and the entire feedback loop, modify within the reducer, the action `LOGIN` is passed and set the user within the state to the one passed within the action, when the `LOGOUT` action is passed, make sure to set the `user` to `null`
12. **Modify the test suites** - Modify the test suites of the different modified components
13. **Understand how to use the Redux Chrome extension** - Install the Redux DevTools extension on your Chrome browser
14. **Combine store: Root reducer** - Since the application has more that one reducer for the application, they will need to be combined in store. Create a new file `reducers/rootReducer.js`, in this file and export a `rootReducer`
15. **Combine store: modify the application** - In `index.js`, create the store using the root reducer instead of only a ui reducer
16. **Combine store: write the tests** - Modify the test suites
17. **Connect notifications: New Action Creator** - Work on connecting a more complex component to the entire API
18. **Connect notifications: Improve reducer** - Make modifications to `notificationReducer` within `notificationReducer.js`
19. **Connect notifications to the reducer** - Make changes to `Notifications.js` component
20. **Connect notifications: clean up** - With the new behavior, clean up old functions and test data
21. **Connect notifications: update the test suites** - Modify the test suites to pass the tests and add new tests
22. **Selectors** - To improve connector performance, always use selectors when you can and modify the Notifications connector to reuse the selector built in the previous project
23. **Connect courses: create a course selector** - In `selector/courseSelector.js`, write a new file `courseSelector.test.js`, that will verify that the selector is working correctly
24. **Connect course: create a fetch course function** - In `actions/courseActionCreators.js`, within `courseActionCreators.test.js`, create a test to verify that the fetch is working correctly
25. **Connect the courses component** - In `CourseList.js` connect the component, create a new function `onChangeRow`, modify `CourseListRow` and in the file `CourseList.test.js` create two new tests
26. **Memoized selectors: Redux Reselect** - Install Redux Reselect and create a new selector named `getUnreadNotificationsByType` in `notificationSelector.js`
27. **Momoized selectors: update the UI** - Make changes in the notifications component
28. **Memoized selectors: update the test suite** - In `Notifications.test.js`, add two new tests, and make updates to `notificationSelector.test.js`
29. **Container/Component** - Use the concept of containers and components
