# myrepos
Display repos from a specified Github account.

# Fetch Vs Axios
In this section, I will be listing our certain features and then I’ll talk about how well Fetch and Axios support these features.

1. Basic Syntax
Both Fetch and Axios have very simple syntaxes for making requests. But Axios has an upper hand because Axios automatically converts a response to JSON, so when using Axios we skip the step of converting the response to JSON, unlike Fetch() where we’d still have to convert the response to JSON. Lastly, Axios shorthand methods allow us to make specific HTTP Requests easier.

1. Browser Compatibility
One of the many reasons why developers would prefer Axios over Fetch is because Axios is supported across major browsers and versions unlike Fetch that is only supported in Chrome 42+, Firefox 39+, Edge 14+, and Safari 10.1+.

1. Handling Response Timeout
Setting a timeout for responses is very easy to do in Axios by making use of the timeout option inside the request object. But in Fetch, it is not that easy to do this. Fetch provides a similar feature by using the AbortController() interface but it takes more time to implement and can get confusing.

1. Intercepting HTTP Requests
Axios allows developers to intercept HTTP requests. HTTP interceptors are needed when we need to change HTTP requests from our application to the server. Interceptors give us the ability to do that without having to write extra code.

1. Making Multiple Requests Simultaneously
Axios allows us to make multiple HTTP requests with the use of the axios.all() method. fetch() provides the same feature with the use of the promise.all() method, we can make multiple fetch() requests inside it.

# Conclusion 
Axios and fetch() are all great ways of consuming APIs but I advise you to use fetch() when building relatively small applications and make use of Axios when building large applications for scalability reasons.
