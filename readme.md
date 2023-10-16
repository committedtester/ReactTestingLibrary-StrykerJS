# GOAL
To confirm the combination of React Testing Library and Mutation Testing

## STEPS
1) Create a basic React Application - DONE
2) Apply React Testing Library with Jest 
3) Use Stryker to identify testing gaps

## HOW TO
* React application created with 'npx create-react-app react-test-example'
* React Testing Library added with npm
* Stryker is executed using 'npm run test'
* Comment out the App.test.js test's lines to see the mutation fail

### Stryker
Note the use of the stryker.config.json file
* We are using the Mutate option to specify which files to mutate 
* We are using the temporary directory to allow stryker to see the test files.
[link](https://github.com/stryker-mutator/stryker-js/blob/master/docs/troubleshooting.md#no-tests-executed---jest-runner)
* We are also using the Ignore Static method to speed up the execution as per
[link](https://stryker-mutator.io/docs/mutation-testing-elements/static-mutants/)
[link](https://stryker-mutator.io/docs/stryker-js/configuration/#ignorestatic-boolean)

