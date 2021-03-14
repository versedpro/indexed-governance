# @indexed-finance/governance

Forked from 
[https://github.com/Uniswap/governance/tree/v1.0.2](https://github.com/Uniswap/governance/tree/v1.0.2)

## Test

> npm run test

## Coverage

> npm run coverage

## Test all

- Make sure that all dependencies are installed. running `yarn`.
- Please add *MAINNET_PVT_KEY, RINKEBY_PVT_KEY, INFURA_PROJECT_ID* into **.env** file.
- Use the scripts in package.json to build, test.
  - order by something like following
    - `yarn prepare-build`
    - `yarn build`
    - `yarn test`
  - You should see success result like this: 
    ```
    ...
    Done in 526.89s.
    ```

## Deploy

- To deploy with proper verification on Etherscan, use the scripts in package.json.
- For example.
  - `yarn deploy:ndx [rinkeby | mainnet]`
- If you face this error, path of source has to contain 'contracts', then you should change source path from 'temp-contracts' to 'contracts'.
- If you run `yarn deploy:ndx`, it will clean temp. so it may cause some errors. In this case, you should run the introductions of command in package.json directly. 
  like this: `yarn deploy:[rinkeby | mainnet] --tags Ndx`