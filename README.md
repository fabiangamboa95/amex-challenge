## Steps & Documentation

- initialized git repository in order to make this code easier to maintain, share and collaborate with others
- .gitignore to exclude unnecessary or unwanted files from the repository
- completed the implementation of the caching fetch library, functional state

## Next Steps I Would Take

- add nodemon to have automatic server restarts on file saved changes
- include .prettierrc.json and .eslintrc.json in order to have a consistent code style and linting
- also add client browser reload on react files saved changes
- include unit tests for the caching fetch library implementation
- maybe also include integration tests with cypress
- configure a CI pipeline, so that the code is automatically tested and deployed on remote repo push
- add monitoring software such as sentry, for production error tracking and logging
- maybe don't do fetch on render, but instead use a store combined with a loading phase to avoid unnecessary re-renders
- from a security standpoint I would encrypt the cached data that is being sent or just use server side rendering to achieve this
- also sanitize the data that is being embedded in the window.__INITIAL_DATA__ to protect against XSS attacks
- I would add auth to the page since the content is user sensitive, since it is providing names, mails and balances
- provide the type interface for the data that is being returned from the API, so that the application can improve type safety