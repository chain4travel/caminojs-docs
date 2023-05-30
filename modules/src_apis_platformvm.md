[@c4tplatform/caminojs](../api.md) › [src/apis/platformvm](src_apis_platformvm.md)

# Module: src/apis/platformvm

## Index

### References

* [ADDRESSSTATECONSORTIUM](src_apis_platformvm.md#addressstateconsortium)
* [ADDRESSSTATEDEFERRED](src_apis_platformvm.md#addressstatedeferred)
* [ADDRESSSTATEKYCVERIFIED](src_apis_platformvm.md#addressstatekycverified)
* [APIDeposit](src_apis_platformvm.md#apideposit)
* [AddDelegatorParams](src_apis_platformvm.md#adddelegatorparams)
* [AddDelegatorTx](src_apis_platformvm.md#adddelegatortx)
* [AddSubnetValidatorTx](src_apis_platformvm.md#addsubnetvalidatortx)
* [AddValidatorParams](src_apis_platformvm.md#addvalidatorparams)
* [AddValidatorTx](src_apis_platformvm.md#addvalidatortx)
* [AddressParams](src_apis_platformvm.md#addressparams)
* [AddressStateTx](src_apis_platformvm.md#addressstatetx)
* [AmountInput](src_apis_platformvm.md#amountinput)
* [AmountOutput](src_apis_platformvm.md#amountoutput)
* [AssetAmountDestination](src_apis_platformvm.md#assetamountdestination)
* [BalanceDict](src_apis_platformvm.md#balancedict)
* [BaseTx](src_apis_platformvm.md#basetx)
* [Blockchain](src_apis_platformvm.md#blockchain)
* [CaminoAddValidatorTx](src_apis_platformvm.md#caminoaddvalidatortx)
* [ClaimAmount](src_apis_platformvm.md#claimamount)
* [ClaimAmountParams](src_apis_platformvm.md#claimamountparams)
* [ClaimTx](src_apis_platformvm.md#claimtx)
* [ClaimType](src_apis_platformvm.md#claimtype)
* [Claimable](src_apis_platformvm.md#claimable)
* [CreateAddressParams](src_apis_platformvm.md#createaddressparams)
* [CreateBlockchainParams](src_apis_platformvm.md#createblockchainparams)
* [CreateChainTx](src_apis_platformvm.md#createchaintx)
* [CreateSubnetParams](src_apis_platformvm.md#createsubnetparams)
* [CreateSubnetTx](src_apis_platformvm.md#createsubnettx)
* [DepositOffer](src_apis_platformvm.md#depositoffer)
* [DepositTx](src_apis_platformvm.md#deposittx)
* [EndIndex](src_apis_platformvm.md#endindex)
* [ExportAVAXParams](src_apis_platformvm.md#exportavaxparams)
* [ExportKeyParams](src_apis_platformvm.md#exportkeyparams)
* [ExportTx](src_apis_platformvm.md#exporttx)
* [GetAllDepositOffersParams](src_apis_platformvm.md#getalldepositoffersparams)
* [GetAllDepositOffersResponse](src_apis_platformvm.md#getalldepositoffersresponse)
* [GetBalanceResponse](src_apis_platformvm.md#getbalanceresponse)
* [GetBalanceResponseAvax](src_apis_platformvm.md#getbalanceresponseavax)
* [GetBalanceResponseCamino](src_apis_platformvm.md#getbalanceresponsecamino)
* [GetClaimablesResponse](src_apis_platformvm.md#getclaimablesresponse)
* [GetConfigurationResponse](src_apis_platformvm.md#getconfigurationresponse)
* [GetCurrentValidatorsParams](src_apis_platformvm.md#getcurrentvalidatorsparams)
* [GetDepositsParams](src_apis_platformvm.md#getdepositsparams)
* [GetDepositsResponse](src_apis_platformvm.md#getdepositsresponse)
* [GetMaxStakeAmountParams](src_apis_platformvm.md#getmaxstakeamountparams)
* [GetMinStakeResponse](src_apis_platformvm.md#getminstakeresponse)
* [GetPendingValidatorsParams](src_apis_platformvm.md#getpendingvalidatorsparams)
* [GetRewardUTXOsParams](src_apis_platformvm.md#getrewardutxosparams)
* [GetRewardUTXOsResponse](src_apis_platformvm.md#getrewardutxosresponse)
* [GetStakeParams](src_apis_platformvm.md#getstakeparams)
* [GetStakeResponse](src_apis_platformvm.md#getstakeresponse)
* [GetTxStatusParams](src_apis_platformvm.md#gettxstatusparams)
* [GetTxStatusResponse](src_apis_platformvm.md#gettxstatusresponse)
* [GetUTXOsParams](src_apis_platformvm.md#getutxosparams)
* [GetUTXOsResponse](src_apis_platformvm.md#getutxosresponse)
* [GetValidatorsAtParams](src_apis_platformvm.md#getvalidatorsatparams)
* [GetValidatorsAtResponse](src_apis_platformvm.md#getvalidatorsatresponse)
* [ImportAVAXParams](src_apis_platformvm.md#importavaxparams)
* [ImportKeyParams](src_apis_platformvm.md#importkeyparams)
* [ImportTx](src_apis_platformvm.md#importtx)
* [KeyChain](src_apis_platformvm.md#keychain)
* [KeyPair](src_apis_platformvm.md#keypair)
* [ListAddressesParams](src_apis_platformvm.md#listaddressesparams)
* [LockedIn](src_apis_platformvm.md#lockedin)
* [LockedOut](src_apis_platformvm.md#lockedout)
* [MultisigAlias](src_apis_platformvm.md#multisigalias)
* [MultisigAliasParams](src_apis_platformvm.md#multisigaliasparams)
* [MultisigAliasReply](src_apis_platformvm.md#multisigaliasreply)
* [MultisigAliasTx](src_apis_platformvm.md#multisigaliastx)
* [Owner](src_apis_platformvm.md#owner)
* [OwnerParam](src_apis_platformvm.md#ownerparam)
* [ParseableInput](src_apis_platformvm.md#parseableinput)
* [ParseableOutput](src_apis_platformvm.md#parseableoutput)
* [PlatformVMAPI](src_apis_platformvm.md#platformvmapi)
* [PlatformVMConstants](src_apis_platformvm.md#platformvmconstants)
* [RegisterNodeTx](src_apis_platformvm.md#registernodetx)
* [SECPCredential](src_apis_platformvm.md#secpcredential)
* [SECPOwnerOutput](src_apis_platformvm.md#secpowneroutput)
* [SECPTransferInput](src_apis_platformvm.md#secptransferinput)
* [SECPTransferOutput](src_apis_platformvm.md#secptransferoutput)
* [SampleValidatorsParams](src_apis_platformvm.md#samplevalidatorsparams)
* [SelectCredentialClass](src_apis_platformvm.md#selectcredentialclass)
* [SelectInputClass](src_apis_platformvm.md#selectinputclass)
* [SelectOutputClass](src_apis_platformvm.md#selectoutputclass)
* [SelectTxClass](src_apis_platformvm.md#selecttxclass)
* [SpendParams](src_apis_platformvm.md#spendparams)
* [SpendReply](src_apis_platformvm.md#spendreply)
* [StakeableLockIn](src_apis_platformvm.md#stakeablelockin)
* [StakeableLockOut](src_apis_platformvm.md#stakeablelockout)
* [StartIndex](src_apis_platformvm.md#startindex)
* [Subnet](src_apis_platformvm.md#subnet)
* [SubnetAuth](src_apis_platformvm.md#subnetauth)
* [TransferableInput](src_apis_platformvm.md#transferableinput)
* [TransferableOutput](src_apis_platformvm.md#transferableoutput)
* [Tx](src_apis_platformvm.md#tx)
* [UTXO](src_apis_platformvm.md#utxo)
* [UTXOID](src_apis_platformvm.md#utxoid)
* [UTXOSet](src_apis_platformvm.md#utxoset)
* [UnlockDepositTx](src_apis_platformvm.md#unlockdeposittx)
* [UnsignedTx](src_apis_platformvm.md#unsignedtx)
* [ValidatorTx](src_apis_platformvm.md#validatortx)
* [WeightedValidatorTx](src_apis_platformvm.md#weightedvalidatortx)

## References

###  ADDRESSSTATECONSORTIUM

• **ADDRESSSTATECONSORTIUM**:

___

###  ADDRESSSTATEDEFERRED

• **ADDRESSSTATEDEFERRED**:

___

###  ADDRESSSTATEKYCVERIFIED

• **ADDRESSSTATEKYCVERIFIED**:

___

###  APIDeposit

• **APIDeposit**:

___

###  AddDelegatorParams

• **AddDelegatorParams**:

___

###  AddDelegatorTx

• **AddDelegatorTx**:

___

###  AddSubnetValidatorTx

• **AddSubnetValidatorTx**:

___

###  AddValidatorParams

• **AddValidatorParams**:

___

###  AddValidatorTx

• **AddValidatorTx**:

___

###  AddressParams

• **AddressParams**:

___

###  AddressStateTx

• **AddressStateTx**:

___

###  AmountInput

• **AmountInput**:

___

###  AmountOutput

• **AmountOutput**:

___

###  AssetAmountDestination

• **AssetAmountDestination**:

___

###  BalanceDict

• **BalanceDict**:

___

###  BaseTx

• **BaseTx**:

___

###  Blockchain

• **Blockchain**:

___

###  CaminoAddValidatorTx

• **CaminoAddValidatorTx**:

___

###  ClaimAmount

• **ClaimAmount**:

___

###  ClaimAmountParams

• **ClaimAmountParams**:

___

###  ClaimTx

• **ClaimTx**:

___

###  ClaimType

• **ClaimType**:

___

###  Claimable

• **Claimable**:

___

###  CreateAddressParams

• **CreateAddressParams**:

___

###  CreateBlockchainParams

• **CreateBlockchainParams**:

___

###  CreateChainTx

• **CreateChainTx**:

___

###  CreateSubnetParams

• **CreateSubnetParams**:

___

###  CreateSubnetTx

• **CreateSubnetTx**:

___

###  DepositOffer

• **DepositOffer**:

___

###  DepositTx

• **DepositTx**:

___

###  EndIndex

• **EndIndex**:

___

###  ExportAVAXParams

• **ExportAVAXParams**:

___

###  ExportKeyParams

• **ExportKeyParams**:

___

###  ExportTx

• **ExportTx**:

___

###  GetAllDepositOffersParams

• **GetAllDepositOffersParams**:

___

###  GetAllDepositOffersResponse

• **GetAllDepositOffersResponse**:

___

###  GetBalanceResponse

• **GetBalanceResponse**:

___

###  GetBalanceResponseAvax

• **GetBalanceResponseAvax**:

___

###  GetBalanceResponseCamino

• **GetBalanceResponseCamino**:

___

###  GetClaimablesResponse

• **GetClaimablesResponse**:

___

###  GetConfigurationResponse

• **GetConfigurationResponse**:

___

###  GetCurrentValidatorsParams

• **GetCurrentValidatorsParams**:

___

###  GetDepositsParams

• **GetDepositsParams**:

___

###  GetDepositsResponse

• **GetDepositsResponse**:

___

###  GetMaxStakeAmountParams

• **GetMaxStakeAmountParams**:

___

###  GetMinStakeResponse

• **GetMinStakeResponse**:

___

###  GetPendingValidatorsParams

• **GetPendingValidatorsParams**:

___

###  GetRewardUTXOsParams

• **GetRewardUTXOsParams**:

___

###  GetRewardUTXOsResponse

• **GetRewardUTXOsResponse**:

___

###  GetStakeParams

• **GetStakeParams**:

___

###  GetStakeResponse

• **GetStakeResponse**:

___

###  GetTxStatusParams

• **GetTxStatusParams**:

___

###  GetTxStatusResponse

• **GetTxStatusResponse**:

___

###  GetUTXOsParams

• **GetUTXOsParams**:

___

###  GetUTXOsResponse

• **GetUTXOsResponse**:

___

###  GetValidatorsAtParams

• **GetValidatorsAtParams**:

___

###  GetValidatorsAtResponse

• **GetValidatorsAtResponse**:

___

###  ImportAVAXParams

• **ImportAVAXParams**:

___

###  ImportKeyParams

• **ImportKeyParams**:

___

###  ImportTx

• **ImportTx**:

___

###  KeyChain

• **KeyChain**:

___

###  KeyPair

• **KeyPair**:

___

###  ListAddressesParams

• **ListAddressesParams**:

___

###  LockedIn

• **LockedIn**:

___

###  LockedOut

• **LockedOut**:

___

###  MultisigAlias

• **MultisigAlias**:

___

###  MultisigAliasParams

• **MultisigAliasParams**:

___

###  MultisigAliasReply

• **MultisigAliasReply**:

___

###  MultisigAliasTx

• **MultisigAliasTx**:

___

###  Owner

• **Owner**:

___

###  OwnerParam

• **OwnerParam**:

___

###  ParseableInput

• **ParseableInput**:

___

###  ParseableOutput

• **ParseableOutput**:

___

###  PlatformVMAPI

• **PlatformVMAPI**:

___

###  PlatformVMConstants

• **PlatformVMConstants**:

___

###  RegisterNodeTx

• **RegisterNodeTx**:

___

###  SECPCredential

• **SECPCredential**:

___

###  SECPOwnerOutput

• **SECPOwnerOutput**:

___

###  SECPTransferInput

• **SECPTransferInput**:

___

###  SECPTransferOutput

• **SECPTransferOutput**:

___

###  SampleValidatorsParams

• **SampleValidatorsParams**:

___

###  SelectCredentialClass

• **SelectCredentialClass**:

___

###  SelectInputClass

• **SelectInputClass**:

___

###  SelectOutputClass

• **SelectOutputClass**:

___

###  SelectTxClass

• **SelectTxClass**:

___

###  SpendParams

• **SpendParams**:

___

###  SpendReply

• **SpendReply**:

___

###  StakeableLockIn

• **StakeableLockIn**:

___

###  StakeableLockOut

• **StakeableLockOut**:

___

###  StartIndex

• **StartIndex**:

___

###  Subnet

• **Subnet**:

___

###  SubnetAuth

• **SubnetAuth**:

___

###  TransferableInput

• **TransferableInput**:

___

###  TransferableOutput

• **TransferableOutput**:

___

###  Tx

• **Tx**:

___

###  UTXO

• **UTXO**:

___

###  UTXOID

• **UTXOID**:

___

###  UTXOSet

• **UTXOSet**:

___

###  UnlockDepositTx

• **UnlockDepositTx**:

___

###  UnsignedTx

• **UnsignedTx**:

___

###  ValidatorTx

• **ValidatorTx**:

___

###  WeightedValidatorTx

• **WeightedValidatorTx**:
