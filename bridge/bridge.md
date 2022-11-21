# Bridge 가이드

## Opening a new way between cryptocurrencies. ​&#x20;

XYLO Bridge 는 서로 다른 네트워크 간의 토큰 교환을 지원하는 서비스 입니다. 현재 구매할 수 있는 TOKEN는 ERC-20 토큰으로 이더리움 메인넷의 토큰입니다. 이더리움 메인넷의 토큰을 XYLO 앱에서 사용하기 위해서는 전송 과정이 필요합니다. XYLO 브릿지를 이용하면 이더리움 TOKEN를 XYLO 메인넷으로 이동시킬 수 있습니다. 네트워크 환경에 따라 약 5분 정도의 시간이 소요되며 이더리움 네트워크 자체에서 발생하는 소량의 수수료가 발생합니다.

XYLO 전용 Bridge는 두 체인 간의 자산을 더 안전하고 빠르게 전송할 수 있는 방법을 제공합니다. 신뢰성 있는 변환을 위해 Hashed Time Lock 기능을 사용하여 보내는 From 네트워크와 받는 To 네트워크 모두 각각의 승인 처리가 필요합니다. 진행 상황이 오래 걸릴 수 있기 때문에 Bridge 화면 또는 익스플로러를 통해 자산 전송 상황을 지속적으로 모니터링 해주시기 바랍니다. 자산 이동은 브라우저용 플러그인(확장 프로그램) 형태의 월렛 연동을 위해 데스크톱 웹에서 가능하며, XYLO Bridge에서 아래의 가이드를 참고해 진행해주세요.

{% hint style="warning" %}
<mark style="color:red;background-color:red;">**만약 100,000 TOKEN이상의 변환을 원하실 경우**</mark> , XYLO Help Center 를 통해 고액자산변환 요청하신 자산변환 진행을 부탁 드립니다.
{% endhint %}



### 메타마스크에 TOKEN 토큰 추가

1. 네트워크(이더리움 메인넷)를 확인합니다.
2. '토큰 가져오기' 클릭합니다.
3. '맞춤형 토큰'을 클릭합니다.
4. 토큰 계약 주소를 입력합니다.&#x20;

```
0x9b9647431632af44be02ddd22477ed94d14aacaa
```

5\. '맞춤형 토큰 추가' 버튼을 클릭합니다.&#x20;

{% hint style="info" %}
토큰 계약 주소를 입력하면 토큰 기호와 토큰 십진수가 자동으로 입력됩니다.
{% endhint %}

6\. TOKEN가 표시되면 '토큰 가져오기' 버튼을 클릭합니다.

7\. TOKEN 토큰 추가가 완료되었습니다.&#x20;

{% hint style="warning" %}
입금 실수 시 TOKEN를 찾을 수 없으니 먼저 소량의 TOKEN 전송 테스트를 해보는 것을 추천합니다.
{% endhint %}



## 이더리움 네트워크 -> 그라운드체인 네트워크&#x20;

### Step 01

1. Asset의 선택 박스를 클릭합니다.
2. Select a coin 팝업이 뜨면 TOKEN 를 선택한 후 Select 버튼을 클릭합니다.

### Step 02

1. From의 선택 박스를 클릭하여 이더리움을 선택합니다.
2. 메타마스크를 선택한 후 OK 버튼을 클릭합니다.

{% hint style="danger" %}
메타마스크의 네트워크가 이더리움 네트워크가 아닐 경우 Network Error경고창이 등장합니다.
{% endhint %}

3\. To의 선택박스를 클릭하여 XYLO Ground Chain을 클릭합니다.

4.XYLO Wallet을 클릭한 후 OK 버튼을 클릭합니다.

5\. XYLO APP 가입 시 생성한 아이디, 비밀번호를 입력합니다. 계정이 없는 경우 XYLO App 회원가입이 필요합니다. 자세한 가입 방법은 Get Started 참고해 주세요.

{% hint style="info" %}
계정이 없는 경우 XYLO App 회원가입이 필요합니다. 자세한 가입 방법은 Get Started 참고해 주세요.
{% endhint %}

6\. To 체인에 대한 Destination이 자동 입력됩니다.

### Step 03

1. 변환할 TOKEN 금액을 입력합니다. 수수료를 제외한 금액을 입력하세요.

{% hint style="danger" %}
최소 전환 수량은 100TOKEN 입니다. 최소 전환 수량보다 적은 수량의 TOKEN를 변환 시도할 경우 경고창이 등장합니다.
{% endhint %}

2\. Convert now 버튼을 클릭합니다.

3\. Check the coin to convert 팝업에서 입력한 내용과 수수료 및 주의사항을 확인한 후 OK 버튼을 클릭합니다.

{% hint style="danger" %}
이더리움 네트워크에서 그라운드체인 네트워크로 변환할 경우 수수료와 Bridge fee 20 TOKEN가 필요합니다.&#x20;
{% endhint %}

{% hint style="info" %}
OK 버튼 클릭 시 최초 1회 데스크탑 알림 설정을 진행합니다. 알림 설정 창이 뜨면 OK버튼을 클릭해 주세요.
{% endhint %}

### Step 04

1. From 체인에 연결된 메타마스크에서 승인 처리를 진행합니다.
2. From 체인에 연결된 메타마스크에서 가스 수수료를 확인합니다. 소량의 이더리움 수수료가 발생됩니다.
3. From 체인 승인처리가 완료되면 트랜잭션이 생성됩니다. 트랜잭션 hash 클릭 시 Explorer로 이동하며 자세한 트랜잭션 정보를 확인할 수 있습니다.
4. Bridge 페이지 내 별도로 생성된 To 체인의 Confirm 버튼을 클릭합니다.
5. Approve 버튼을 클릭하여 To 체인의 승인 처리를 진행합니다.
6. To 체인 승인 처리가 완료되면 트랜잭션을 확인할 수 있습니다. 최종 변환이 완료되었습니다.

{% hint style="info" %}
XYLO APP의 Wallet 페이지에서 전송된 KOK를 확인할 수 있습니다.
{% endhint %}

## 그라운드체인 네트워크 -> 이더리움 네트워크

### Step 01

1. Asset의 선택 박스를 클릭합니다.
2. Select a coin 팝업이 뜨면 KOK를 선택한 후 Select 버튼을 클릭합니다.

### Step 02

1. From의 선택 박스를 클릭하여 XYLO GroundChain을 선택합니다.
2. XYLO Wallet을 선택한 후 OK 버튼을 클릭합니다.
3. XYLO APP 가입 시 생성한 아이디, 비밀번호를 입력합니다.
4. To의 선택박스를 클릭하여 이더리움을 선택합니다.
5. 메타마스크를 선택한 후 OK 버튼을 클릭합니다.
6. To 체인에 대한 Destination이 자동 입력됩니다.

### Step 03

1. 변환할 TOKEN 금액을 입력합니다. 수수료를 제외한 금액을 입력하세요.

{% hint style="danger" %}
최소 전환 수량은 100TOKEN 입니다. 최소 전환 수량보다 적은 수량의 TOKEN를 변환 시도할 경우 경고창이 등장합니다.
{% endhint %}

2\. Convert now 버튼을 클릭합니다.

3\. Check the coin to convert 팝업에서 입력한 내용과 수수료 및 주의사항을 확인한 후 OK 버튼을 클릭합니다.

{% hint style="danger" %}
그라운드 체인 네트워크에서 이더리움 네트워크로 변환할 경우 수수료와 Bridge fee 30 TOKEN가 필요합니다.
{% endhint %}

{% hint style="info" %}
OK 버튼 클릭 시 최초 1회 데스크탑 알림 설정을 진행합니다. 알림 설정 창이 뜨면 동의해 주세요.
{% endhint %}



### Step 04

1. From 체인에 연결된 Confirm 버튼을 클릭합니다.
2. From 체인에 Approve 버튼을 클릭합니다.
3. From 체인 승인 처리가 완료되면 트랜잭션이 생성됩니다. 트랜잭션 hash 클릭 시 Explorer로 이동하며 자세한 트랜잭션 정보를 확인할 수 있습니다.
4. To 체인의 메타마스크 인증을 진행합니다.
5. 최종 변환이 완료 되었습니다.



## 히스토리 확인

1. History 메뉴 또는 우상단 Transaction으로 이동하여 트랜잭션 상태를 확인할 수 있습니다.

#### 히스토리 상태&#x20;

{% tabs %}
{% tab title="완료 " %}
작업이 성공적으로 완료되었습니다.
{% endtab %}

{% tab title="승인 필요" %}
To 체인에 연결된 지갑에서 트랜잭션 승인이 필요한 상태입니다. Confirm 버튼을 클릭하여 승인 처리를 진행합니다.
{% endtab %}

{% tab title="진행중" %}
현재 트랜잭션이 진행 중인 상황으로, 전환이 완료 상태로 변경될 때까지 대기합니다.
{% endtab %}

{% tab title="실패" %}
Timeout 또는 To 체인에 연결된 지갑에서 전송에 실패한 상태로 Refund 버튼을 클릭하여 환불을 진행합니다.
{% endtab %}
{% endtabs %}

## 오류시 대처 방법

### 브릿지 사용 중 오류 발생 시&#x20;

브릿지 사용 중 오류 발생 시 상단 History에서 나의 모든 TOKEN 전환 내역을 확인 가능합니다. 전송 중 Confirm 버튼을 클릭하지 못한 경우 History에서 전환 중 누르지 못한 Confirm을 진행할 수 있습니다.&#x20;

또한 Confirm을 48시간 동안 누르지 않을 경우 환불 절차가 진행되며 History에서 해당 절차를 확인하실 수 있습니다.
