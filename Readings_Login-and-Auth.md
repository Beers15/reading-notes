[Home](README.md)
 
# Readings: \<Login /\> and \<Auth /\>
 
## Review, Research, and Discussion
 
---------------
All answers taken from resources supplied in prompt

1) Why is the Context API useful?

  * It allows us to create global state that can easily be accessed from any level of a component tree without having to resort to passing props and state down or more complex state management libraries such as Redux.

2) Can a component outside of a provider get its context?

  * This cannot be done. A component or one of its parent components higher in its own component tree must be wrapped in a provider of a given context if it is to access that context's values. 

3) What are some common use cases for using the Context API?

  * Managing theme, configuration, authorization + authentication, and user preference related data are some common cases for using this API. 

4) Describe “Context Hell”

  * This is similar to callback hell. When multiple contexts are wrapping some component, it can get quite ugly. Here is one example from the resource below<sup>1</sup> that illustrates this problem.

  ```javascript
    <>
     <ReduxProvider value={store}>
      <ThemeProvider value={theme}>
       <OtherProvider value={otherValue}>
        <OtherOtherProvider value={otherOtherValue}>
         {/** ... other providers*/}
                                <HellProvider value={hell}>
                                  <HelloWorld />
                                </HellProvider>
         {/** ... other providers*/}
        </OtherOtherProvider>
       </OtherProvider>
      </ThemeProvider>
     </ReduxProvider>
    </>
  ```

### Vocabulary terms

global state

  * This is state that is available anywhere in a Component tree without having to be passed down from component to component. React Context is way way to achieve global state.

global context

  * A context that wraps an entire React app, or large part of a React app could be considered this. Global context can provide its values to any consumer within that component tree. 

provider

  * In the React Context API, the context provider wraps another component and serves its values to that component.

consumer

  * In the React Context API, a consumer of a given context is a descendant of that context's provider. Consumers will re-render whenever the values from that context experience change. They will have access to the global state-like values from that provider.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?

    * Context API
    * Provider + Consumer design pattern
    * cookies

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Implementing different types of contexts in a single application to simplify the process of passing around of state values
    * Ways to prevent "callback hell"
    * Using react-cookies
 
3) What are you most excited about trying to implement or see how it works?
 
    * Implementing an auth related Context Provider in an application

--------------

### Resources

<sup>1</sup> https://dev.to/alfredosalzillo/the-react-context-hell-7p4

https://reactjs.org/docs/context.html#contextprovider

https://www.npmjs.com/package/react-cookies

https://www.npmjs.com/package/react-cookie

https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more