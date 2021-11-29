Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **ERC20Properties** | Interface |  |||
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | name | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
||||||
| **ERC20Clone** | Interface |  |||
| └ | mintbyControl | External ❗️ | 🛑  |NO❗️ |
| └ | burnbyControl | External ❗️ | 🛑  |NO❗️ |
||||||
| **AbsERC20Factory** | Interface |  |||
| └ | createStorage | External ❗️ | 🛑  |NO❗️ |
||||||
| **Controller** | Implementation | Initializable, UUPSUpgradeable, OwnableUpgradeable |||
| └ | isKilled | Internal 🔒 |   | |
| └ | kill | External ❗️ | 🛑  | onlyOwner |
| └ | revive | External ❗️ | 🛑  | onlyOwner |
| └ | initialize | Public ❗️ | 🛑  | initializer |
| └ | _authorizeUpgrade | Internal 🔒 | 🛑  | onlyOwner |
| └ | setFactory | External ❗️ | 🛑  | onlyOwner |
| └ | setProposalContract | External ❗️ | 🛑  | onlyOwner |
| └ | createBulkDerivative | External ❗️ | 🛑  | noReentrant |
| └ | _updateMappings | Internal 🔒 | 🛑  | |
| └ | _safeTransferERC20 | Internal 🔒 | 🛑  | |
| └ | _deployNewERC20 | Internal 🔒 | 🛑  | |
| └ | _mintWrappedTokens | Internal 🔒 | 🛑  | |
| └ | tokenTransfer | External ❗️ | 🛑  |NO❗️ |
| └ | withdrawToken | External ❗️ | 🛑  | noReentrant |
| └ | _timestampToDate | Internal 🔒 |   | |
| └ | _uint2str | Internal 🔒 |   | |
| └ | getS | Public ❗️ |   |NO❗️ |
||||||
| **TimestampToDateLibrary** | Library |  |||
| └ | _daysToDate | Internal 🔒 |   | |
| └ | timestampToDate | Internal 🔒 |   | |
||||||
| **Initializable** | Implementation |  |||
||||||
| **UUPSUpgradeable** | Implementation | Initializable, ERC1967UpgradeUpgradeable |||
| └ | __UUPSUpgradeable_init | Internal 🔒 | 🛑  | initializer |
| └ | __UUPSUpgradeable_init_unchained | Internal 🔒 | 🛑  | initializer |
| └ | upgradeTo | External ❗️ | 🛑  | onlyProxy |
| └ | upgradeToAndCall | External ❗️ |  💵 | onlyProxy |
| └ | _authorizeUpgrade | Internal 🔒 | 🛑  | |
||||||
| **ERC1967UpgradeUpgradeable** | Implementation | Initializable |||
| └ | __ERC1967Upgrade_init | Internal 🔒 | 🛑  | initializer |
| └ | __ERC1967Upgrade_init_unchained | Internal 🔒 | 🛑  | initializer |
| └ | _getImplementation | Internal 🔒 |   | |
| └ | _setImplementation | Private 🔐 | 🛑  | |
| └ | _upgradeTo | Internal 🔒 | 🛑  | |
| └ | _upgradeToAndCall | Internal 🔒 | 🛑  | |
| └ | _upgradeToAndCallSecure | Internal 🔒 | 🛑  | |
| └ | _getAdmin | Internal 🔒 |   | |
| └ | _setAdmin | Private 🔐 | 🛑  | |
| └ | _changeAdmin | Internal 🔒 | 🛑  | |
| └ | _getBeacon | Internal 🔒 |   | |
| └ | _setBeacon | Private 🔐 | 🛑  | |
| └ | _upgradeBeaconToAndCall | Internal 🔒 | 🛑  | |
| └ | _functionDelegateCall | Private 🔐 | 🛑  | |
||||||
| **IBeaconUpgradeable** | Interface |  |||
| └ | implementation | External ❗️ |   |NO❗️ |
||||||
| **AddressUpgradeable** | Library |  |||
| └ | isContract | Internal 🔒 |   | |
| └ | sendValue | Internal 🔒 | 🛑  | |
| └ | functionCall | Internal 🔒 | 🛑  | |
| └ | functionCall | Internal 🔒 | 🛑  | |
| └ | functionCallWithValue | Internal 🔒 | 🛑  | |
| └ | functionCallWithValue | Internal 🔒 | 🛑  | |
| └ | functionStaticCall | Internal 🔒 |   | |
| └ | functionStaticCall | Internal 🔒 |   | |
| └ | verifyCallResult | Internal 🔒 |   | |
||||||
| **StorageSlotUpgradeable** | Library |  |||
| └ | getAddressSlot | Internal 🔒 |   | |
| └ | getBooleanSlot | Internal 🔒 |   | |
| └ | getBytes32Slot | Internal 🔒 |   | |
| └ | getUint256Slot | Internal 🔒 |   | |
||||||
| **OwnableUpgradeable** | Implementation | Initializable, ContextUpgradeable |||
| └ | __Ownable_init | Internal 🔒 | 🛑  | initializer |
| └ | __Ownable_init_unchained | Internal 🔒 | 🛑  | initializer |
| └ | owner | Public ❗️ |   |NO❗️ |
| └ | renounceOwnership | Public ❗️ | 🛑  | onlyOwner |
| └ | transferOwnership | Public ❗️ | 🛑  | onlyOwner |
| └ | _setOwner | Private 🔐 | 🛑  | |
||||||
| **ContextUpgradeable** | Implementation | Initializable |||
| └ | __Context_init | Internal 🔒 | 🛑  | initializer |
| └ | __Context_init_unchained | Internal 🔒 | 🛑  | initializer |
| └ | _msgSender | Internal 🔒 |   | |
| └ | _msgData | Internal 🔒 |   | |
||||||
| **SafeERC20Upgradeable** | Library |  |||
| └ | safeTransfer | Internal 🔒 | 🛑  | |
| └ | safeTransferFrom | Internal 🔒 | 🛑  | |
| └ | safeApprove | Internal 🔒 | 🛑  | |
| └ | safeIncreaseAllowance | Internal 🔒 | 🛑  | |
| └ | safeDecreaseAllowance | Internal 🔒 | 🛑  | |
| └ | _callOptionalReturn | Private 🔐 | 🛑  | |
||||||
| **IERC20Upgradeable** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |


 Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
