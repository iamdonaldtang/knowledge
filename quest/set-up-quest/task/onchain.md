# OnChain

Tasks include holding, swapping, providing liquidity, lending, staking, and identity verification.

TaskOn’s backend currently organizes tasks into sectors such as General, DEX, Lending, and Bridge. Available OnChain task templates include `Wallet Balance`, `Smart Contract`, `Gas Related`, `Uniswap`, `Pancakeswap`, `Curve`, `Metis`, `Nibiru`, `Chainge`, `AAVE`, `Compound`, `Raydium`, `Aerodrome`, and `Task Aggregator`.

In the **General** sector, the platform provides templates for Wallet Balance, Smart Contract, Gas, as well as modules for Metis, Core, Nibiru, and Name Service (e.g., ENS Hold).

The **Smart Contract** template is the most commonly used, enabling task interactions (e.g., transfers, swaps, adding liquidity, lending) on a specified network and smart contract. The platform automates verification.

### To set up:

* Specify the task name, select the network address, choose the smart contract, provide the URL for user access, and set the time range for contract interaction (defaults to the task’s duration). Finally, include task instructions explaining how to complete it.
* After selecting a network, some commonly used contracts are pre-integrated into the template, allowing you to check if the desired contract is available. Contracts must be whitelisted to be used; if not listed, you can apply for whitelisting in the backend.

This task template corresponds to the API and supports automated verification through the contract module, offering a more intelligent approach.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdgaFIwzqbCHGLk2hu1EPOULruhGBIRpymfcza6G7q7aagvRytQZiouqmKT9mJmX4KFrTAj7ILIp2qdRHX91pDNPsxNdAddgkOWRk1cpGqZYB_5PWxlq9Xit2FqxMZdTIXNkIGxDA?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd-xA0UZBYII1IEUgED407Mr0OKcO_e4BSKuI1fPXFsAEZd8OF_spgaBSp3silLOOOZebtInsmzPqwdzbtMEykDl3wCq3yUUlifzTqt-W2Xj9Y5TpMc4t7oBKyciFRuooZ6HoE1sQ?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

For **Identity Verification**, the Wallet Balance template allows you to restrict tasks to users holding specific tokens or NFTs.

The **Gas Related Task** template enables on-chain identity verification:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcBwgETZdV_gVk5iZ9C1pp_I19IgJ9y2QjIf3CDdDBQBeprZyml_LrrfsaTyXGbNCxnNtpH6R9N11NFndenssNCst7xYidlVw2dbKI8nEep-ZumpaqjKv6_i8kn4u9qG9b9ZgqM3A?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

**Gas Fee Spent Amount**:&#x20;

Checks the amount of gas fees spent by users on a specified chain. You can set a minimum gas fee threshold to filter eligible on-chain users for the task and define the verification time frame (e.g., interaction records within a certain number of days).

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeq-eoSamiuV-EeV7Biu6xNVlgqYsntxdnoEo2qgxlvedGdOdptJsM7ZCW66i_5I9mZTVzmfHbwGk2nejArQUHSkoQM-OWYYb0WWzvx1veQGr-DsR0Gsc4xKFSaABEYVVTwUgkwyw?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

**Number of Transactions on a Specified Chain**:&#x20;

Verifies if users meet the required number of transactions on a specified chain. You can set a minimum transaction count to filter eligible users and define the verification time frame (e.g., interaction records within a certain number of days).

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcD422z74l8bswByLE-at3McYWiUNBXOp0-qRns9jgli-AghgLtMCyy92loaN4kAWhza_XBQ40mlMGZpPyjDBzTVKyZcl3hylek1SQuhgvHHKtV8PpFIoDhPZR_Sw9EomwmWMhEHw?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

**DEX Sector:**

Includes platforms like `TaskOn Aggregator`, `Uniswap`, `Pancakeswap`, `Curve`, `Raydium`, `Chainge`, and `Aerodrome`.

**Lending Sector**:\
Includes platforms like `AAVE` and `Compound`.

**Bridge Sector:**

Includes platforms like `Metis`.



Based on your OnChain task requirements, select the appropriate network, token, and platform (Swap, DEX, Lending, Bridge) for task setup.

Notably, OnChain contract interaction tasks can be configured via smart contracts to set up tasks related to liquidity, lending, supplying, mining, and swapping—any task based on smart contracts.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXei8TCSpseB3dFuesLwbePIo5ChC-HgPKRjkrPWzvnqwBlOEk8fDvv4HIk4dIL3QTTc97PpFsw79F2nMbU4MmJK4jSd61A4dLf7LVNGsRu3olwEPjtWxYYNyvApqOefcNaJnubQ?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>
