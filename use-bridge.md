# Use Bridge

### Opening a new way between cryptocurrencies

K STADIUM is a service that supports token exchange between different networks. Currently KOK is on the ERC-20 network and is an Ethereum based Mainnet token. In order to use Ethereum mainnet tokens in the XYLO app, a conversion process is required. With the XYLO bridge, Ethereum KOK can be moved to the XYLO mainnet. Depending on the network environment, it takes about 5 minutes and a small fee will be incurred by the Ethereum network itself.

The XYLO specific Bridge provides a safer and faster way to transfer assets between two chains. For reliable conversion, XYLO Bridge uses the HashedTimeLock feature. Both the From network and To network require respective authorization processes. As the process may take a long time, please continue to monitor the transfer of assets through the Bridge screen or Explorer. The asset can be moved from the desktop web by connecting the wallet in the form of a browser plug-in, and please refer to the guide below at XYLO bridge.&#x20;

{% hint style="warning" %}
<mark style="color:red;background-color:red;">If you want to convert more than 100,000 KOK,</mark> please contact us through the XYLO Help Center before proceeding with the conversion.
{% endhint %}

#### Add KOK token to Metamask

1. Check the network (Ethereum Mainnet).
2. Click Import tokens.
3. Select the Custom Token tab.
4. Enter the Token Contract Address.&#x20;

```
0x9b9647431632af44be02ddd22477ed94d14aacaa
```

5\. Click the Add Custom Token button.&#x20;

{% hint style="info" %}
When you enter the Token Contract Address, the Token Symbol and Token Decimal are automatically entered.
{% endhint %}

6\. Click the Import Tokens button.

7\. Added KOK token.&#x20;

{% hint style="warning" %}
If you make an incorrect deposit, you can’t find KOK, so it is recommended to test conversion with a small amount of KOK first.
{% endhint %}



### Ethereum -> Groundchain conversion&#x20;

#### Step 01

1. Click the Asset select box.
2. If the Select coin window pops up, select KOK and click the Select button.

#### Step 02

1. Click the From select box and select Ethereum.
2. Select Metamask and click the OK button.&#x20;

{% hint style="danger" %}
Network Error message pops up when your Metamask network isn't on the Ethereum mainnet.
{% endhint %}

3\. Click the To select box and select XYLO\_Ground Chain.

4\. Select the XYLO Wallet and click the OK button.

5\. Enter the ID and password created when signing up for the XYLO app.&#x20;

{% hint style="info" %}
If you don't have an account, you need to sign up. Please refer to the Get Started for more information on signing up.
{% endhint %}

6\. Destination for the To chain is automatically entered.

#### Step 03

1. Enter the amount of KOK to convert. Enter the amount excluding the fee.&#x20;

{% hint style="danger" %}
The minimum conversion amount is 100KOK.&#x20;

In case of converting amount less than minimum amount, Error message pops up.
{% endhint %}

2\. Click the Convert button.

3\. On the Check the coin to convert pop-up, check the contents entered, fees, and precautions, and click the OK button.&#x20;

{% hint style="danger" %}
In case of conversion from Ethereum to Groundchain, a tax and 20 KOK bridge fees are charged.&#x20;
{% endhint %}

{% hint style="info" %}
Clicking OK button, you need to set the desktop notification for the first time. If the notification settings window appears, please accept it.
{% endhint %}

#### Step 04

1. Proceed with the confirmation process on Metamask connected to the From chain. A small amount of Ethereum gas cost occurs.
2. Check the gas fee on the Metamask connected to From Chain. A small amount of Ethereum gas cost occurs.
3. When the From chain approval process is completed, a transaction is created. When you click on the transaction hash, you can go to Explorer for more transaction information.
4. On the Bridge page, click the Confirm button which is separately created To chain.
5. Click the Approve button to proceed approval action of To Chain.
6. After approval of To chain, you can check the transaction.&#x20;

{% hint style="info" %}
Conversion is completed. You can check converted KOK on the Wallet page of XYLO APP.
{% endhint %}



### Groundchain -> Ethereum conversion&#x20;

#### Step 01

1. Click the Asset select box.
2. If the Select coin window pops up, select KOK and click the Select button.

#### Step 02

1. Click the From select box and select KSTADIUM GroundChain.
2. Select K STADIUM Wallet and click the OK button.
3. Enter the ID and password created when signing up for the XYLO app.
4. Click the To select box and select Ethereum Chain.
5. Select Metamask and click the OK button.
6. Destination for the To chain is automatically entered.

#### Step 03

1. Enter the amount of KOK to convert.&#x20;

{% hint style="danger" %}
Enter the amount excluding the fee. The minimum conversion amount is 100KOK. In case of converting amount less than minimum amount, Error message pops up.
{% endhint %}

2\. Click the Convert button.

3\. On the Check the coin to convert pop-up, check the contents entered, fees, and precautions, and click the OK button.&#x20;

{% hint style="warning" %}
In case of conversion from Groundchain to Ethereum, a tax and 30 KOK bridge fees are charged.&#x20;
{% endhint %}

{% hint style="info" %}
Clicking OK button, you need to set the desktop notification for the first time. If the notification settings window appears, please accept it.
{% endhint %}

#### Step 04

1. On the Bridge page, click the Confirm button which is separately created.
2. Click the Approve button to proceed approval action of sending Chain.
3. When the From chain approval process is completed, a transaction is created. When you click on the transaction hash, you can go to Explorer for more transaction information.
4. Proceed with the confirmation process on Metamask connected to the receiving chain.
5. Conversion is completed.

#### Checking History

1. You an check transaction state by going to the History menu.

#### History state&#x20;

{% tabs %}
{% tab title="Complete" %}
Conversion is successfully completed.
{% endtab %}

{% tab title="approval needed " %}
Transaction authorization is required from the wallet connected to the To chain. Click Confirm to proceed with the approval process.
{% endtab %}

{% tab title="pending" %}
The transaction is currently in progress. Wait for the transition to be changed to a complete state.
{% endtab %}

{% tab title="Failed" %}
Timeout or fail to convert in the wallet connected to the To chain. Click the Refund button to proceed with the refund.
{% endtab %}
{% endtabs %}

### In case of conversion failure&#x20;

#### Conversion failed when using the Bridge&#x20;

In case of conversion failure or unexpected error when using the Bridge, you can check all your KOK conversion history in the History menu.&#x20;

You can proceed confirmation by clicking Confirm button in the History. In addition, you can get a refund 48 hours after Confirm button appears.
