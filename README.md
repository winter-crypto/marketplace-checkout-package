# @usewinter/checkout
:rocket::rocket:  React package to integrate Winter checkout :rocket::rocket:

🚨Note: Depending on your marketplace's smart contracts, this integration may differ. Please contact us at `marketplaces@usewinter.com` and we can help you!

Installation
```
npm i winter-marketplace-checkout

OR 

yarn add winter-marketplace-checkout
```

Usage in your react app
```
import { WinterCheckout } from 'winter-marketplace-checkout';


<WinterCheckout
  showModal={showWinterModal}
  walletAddress={account.isConnected ? account.address : undefined}
  contractAddress={clickedContractAddress}
  tokenId={clickedTokenId}
  production={process.env.WINTER_ENV == 'production' ? true : false }
  onClose={() => {
    setShowWinterModal(false)
  }}
/>

```

### Params:

#### PRODUCTION
false if you're testing in sandbox, true when you go live! 

#### showModal
this toggles true / false based on the state of your "Pay with Card" button
