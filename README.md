# experiment-treeshake-directlinejs

Experiment on tree-shaking botframework-directlinejs

## How to setup/run

Initially, `cd component && npm install`.

For subsequent runs, `npm test`.

## Observations

When importing from the root, it will import `botframework-directlinejs`, but not using it.

When importing from named exports, it will not import `botframework-directlinejs` at all.

![image](https://user-images.githubusercontent.com/1622400/219450166-5935eea4-4646-4f41-bfc1-fe7522faf990.png)

As in the table above, just importing `botframework-directlinejs` incur costs, even without using it.
