



##### [Back to Platform docs](./README.md)

## Customer Methods
Authentication Service
* [verify](#verify)
* [resendPaymentRequest](#resendpaymentrequest)
* [createOrder](#createorder)
* [link](#link)
* [unlink](#unlink)
* [getAccessToken](#getaccesstoken)
* [renewAccessToken](#renewaccesstoken)
* [refund](#refund)
* [refundStatus](#refundstatus)
* [getSchemes](#getschemes)
* [checkEligibility](#checkeligibility)



## Methods with example and description


### verify
Verify Customer



```javascript
// Promise
const promise =  
        customer.verify(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.verify(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [VerifyCustomer](#VerifyCustomer) | yes | Request body |


Use this API to verify the customer based on  mobile number and countryCode.

*Returned Response:*




[VerifyCustomerSuccess](#VerifyCustomerSuccess)

Success. Returns a JSON object as shown below. Refer `VerifyCustomerSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; status</i></summary>

```json
"enabled"
```
</details>

</details>









---


### resendPaymentRequest
Resend Payment Request



```javascript
// Promise
const promise =  
        customer.resendPaymentRequest(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.resendPaymentRequest(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [ResendPaymentRequest](#ResendPaymentRequest) | yes | Request body |


Use this API to resend payment request to user

*Returned Response:*




[CreateTransactionSuccess](#CreateTransactionSuccess)

Success. Returns a JSON object as shown below. Refer `CreateTransactionSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; redirectUrl</i></summary>

```json
"https://account.potleex0.de/auth/login?onboardingToken=e738521b-a763-460d-a440-d9570e79be47&redirectUrl=https://local.potleex0.de:3003/callback?apiKey=0c8e7bbf-6c0c-41b1-8a37-7e066e8fbd4a&apiSecret=48a7d96f46868f78297be845b6afb5da50893d0b&domain=https://api.potleex0.de"
```
</details>

<details>
<summary><i>&nbsp; message</i></summary>

```json
"Payment Authorised"
```
</details>

<details>
<summary><i>&nbsp; userStatus</i></summary>

```json
"PAYMENT_AUTHORISED"
```
</details>

</details>









---


### createOrder
Create Order



```javascript
// Promise
const promise =  
        customer.createOrder(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.createOrder(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [CreateTransaction](#CreateTransaction) | yes | Request body |


Use this API to create transaction for user

*Returned Response:*




[CreateTransactionSuccess](#CreateTransactionSuccess)

Success. Returns a JSON object as shown below. Refer `CreateTransactionSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; chargeToken</i></summary>

```json
"19be735d-5a4a-4c44-8f2b-d640f7509c4d"
```
</details>

<details>
<summary><i>&nbsp; transactionId</i></summary>

```json
"6b5e3348-23b0-43cb-af98-37d603385369"
```
</details>

</details>









---


### link
Link account



```javascript
// Promise
const promise =  
        customer.link(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.link(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [LinkAccount](#LinkAccount) | yes | Request body |


Use this API to link account with merchant

*Returned Response:*




[LinkAccountSuccess](#LinkAccountSuccess)

Success. Returns a JSON object as shown below. Refer `LinkAccountSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; redirectUrl</i></summary>

```json
"https://account.potlee.co.in/auth/login?linkingToken=1245rtfyg765"
```
</details>

</details>









---


### unlink
Unlink account



```javascript
// Promise
const promise =  
        customer.unlink(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.unlink(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [UnlinkAccount](#UnlinkAccount) | yes | Request body |


Use this API to unlink account from merchant

*Returned Response:*




[UnlinkAccountSuccess](#UnlinkAccountSuccess)

Success. Returns a JSON object as shown below. Refer `UnlinkAccountSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; success</i></summary>

```json
true
```
</details>

</details>









---


### getAccessToken
Get Access Token



```javascript
// Promise
const promise =  
        customer.getAccessToken(
            
            
        
        );

// Async/Await
const data = await 
                    customer.getAccessToken(
                    
                    
                    );
```






Use this API to get access token

*Returned Response:*




[GetAccessTokenResponse](#GetAccessTokenResponse)

Success. Returns a JSON object as shown below. Refer `GetAccessTokenResponse` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; success</i></summary>

```json
true
```
</details>

<details>
<summary><i>&nbsp; accessToken</i></summary>

```json
"oa-0a7a064dd15ef22fe002946f90c1e7b22eea47de"
```
</details>

<details>
<summary><i>&nbsp; refreshToken</i></summary>

```json
"oa-d2f33b6be9957050386be051501b84b008f5ef6f"
```
</details>

<details>
<summary><i>&nbsp; tokenExpireAt</i></summary>

```json
"2023-06-27T09:43:07.818Z"
```
</details>

<details>
<summary><i>&nbsp; tokenExpiryIn</i></summary>

```json
"600"
```
</details>

<details>
<summary><i>&nbsp; refreshTokenExpiryAt</i></summary>

```json
"2023-06-27T10:33:07.822Z"
```
</details>

<details>
<summary><i>&nbsp; refreshTokenExpiryIn</i></summary>

```json
"3600"
```
</details>

<details>
<summary><i>&nbsp; scope</i></summary>

```json
[
  "transaction"
]
```
</details>

</details>









---


### renewAccessToken
Renew Access Token



```javascript
// Promise
const promise =  
        customer.renewAccessToken(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.renewAccessToken(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [RefreshTokenRequest](#RefreshTokenRequest) | yes | Request body |


Use this API to renew access token

*Returned Response:*




[RefreshTokenResponse](#RefreshTokenResponse)

Success. Returns a JSON object as shown below. Refer `RefreshTokenResponse` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; success</i></summary>

```json
true
```
</details>

<details>
<summary><i>&nbsp; accessToken</i></summary>

```json
"oa-de1496c16c91c45396ba87a888eed20fb223995d"
```
</details>

<details>
<summary><i>&nbsp; tokenExpireAt</i></summary>

```json
"2023-06-26T19:23:46.977Z"
```
</details>

<details>
<summary><i>&nbsp; tokenExpiryIn</i></summary>

```json
"600"
```
</details>

</details>









---


### refund
Refund customer order amount



```javascript
// Promise
const promise =  
        customer.refund(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.refund(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [Refund](#Refund) | yes | Request body |


Use this API to verify the refund customer order amount

*Returned Response:*




[VerifyCustomerSuccess](#VerifyCustomerSuccess)

Success. Returns a JSON object as shown below. Refer `RefundSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; status</i></summary>

```json
"enabled"
```
</details>

</details>









---


### refundStatus
Refund status



```javascript
// Promise
const promise =  
        customer.refundStatus(
            { 
             refundId : value,
             orderId : value
            
         }
        );

// Async/Await
const data = await 
                    customer.refundStatus(
                    { 
                      refundId : value,
                      orderId : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |  
| refundId | string | no | This is the refundId |    
| orderId | string | no | This is the order ID |  



Use this API to fetch the refund status

*Returned Response:*




[RefundStatus](#RefundStatus)

Success. Returns a JSON object as shown below. Refer `RefundStatus` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; orderId</i></summary>

```json
"PM-28"
```
</details>

<details>
<summary><i>&nbsp; userId</i></summary>

```json
"c004a863-bce5-492b-b7aa-ba2890bc9e25"
```
</details>

<details>
<summary><i>&nbsp; merchantId</i></summary>

```json
"3e0cf7da-ad5f-4c99-a9e7-49cad484ef37"
```
</details>

<details>
<summary><i>&nbsp; lenderId</i></summary>

```json
"f622b3e8-c797-434d-948f-d0fda56e3db6"
```
</details>

<details>
<summary><i>&nbsp; refund</i></summary>

```json
[
  {
    "id": "10122313672606485999",
    "loanAccountNumber": "CASHe-1686764747795",
    "orderItems": {
      "list": [
        {
          "sku": "1",
          "rate": "1",
          "category": "1",
          "quantity": 1
        }
      ]
    },
    "amount": 3000,
    "status": "SUCCESS",
    "processedDate": "2023-06-14T17:44:28.052Z",
    "createdAt": "2023-06-14T17:44:28.052Z"
  }
]
```
</details>

</details>









---


### getSchemes
Fetch schemes



```javascript
// Promise
const promise =  
        customer.getSchemes(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.getSchemes(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [VerifyCustomer](#VerifyCustomer) | yes | Request body |


Use this API to fetch available schemes for user order.

*Returned Response:*




[GetSchemesSuccess](#GetSchemesSuccess)

Success. Returns a JSON object as shown below. Refer `GetSchemesSuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; userId</i></summary>

```json
"bf94b96a-1a15-406b-8d2f-0b37bfe47732"
```
</details>

<details>
<summary><i>&nbsp; lenders</i></summary>

```json
[
  {
    "id": "315f60f4-1238-462c-8108-cfff9fbc400f",
    "name": "CASHe",
    "title": "CASHe",
    "subtitle": "Bhanix Finance and Investment Limited",
    "isDefault": false,
    "logoUrl": "https://cdn.pixelbin.io/v2/potlee/original/public/lenders/lenderLogo/v2/512h-logo/cashe-logo.png",
    "amount": 5000,
    "paymentOptions": {
      "emis": [
        {
          "id": 62,
          "title": "3 Months - EMIs",
          "subtitle": "CASHe Shop 3EMI (PaymentGateway)",
          "description": "3 Months - No cost EMIs",
          "tenure": 3,
          "interest": 0,
          "processingFee": 75,
          "amount": 1692,
          "emiSchedule": [
            {
              "installmentNo": 1,
              "installmentAmount": 1741,
              "dueDate": "2023-12-22T12:00:00.000+00:00",
              "dueAmount": 3334
            },
            {
              "installmentNo": 2,
              "installmentAmount": 1666,
              "dueDate": "2024-01-22T12:00:00.000+00:00",
              "dueAmount": 1668
            },
            {
              "installmentNo": 3,
              "installmentAmount": 1666,
              "dueDate": "2024-02-22T12:00:00.000+00:00",
              "dueAmount": 2
            }
          ],
          "isDefault": false
        }
      ],
      "payLater": {
        "id": 1,
        "title": "PayLater",
        "subtitle": "CASHe_PayLater",
        "description": "Customer can pay after 30days",
        "tenure": 1,
        "interest": 0,
        "processingFee": 0,
        "amount": 5000,
        "emiSchedule": null,
        "isDefault": true
      }
    }
  }
]
```
</details>

</details>









---


### checkEligibility
Check Credit Eligibility



```javascript
// Promise
const promise =  
        customer.checkEligibility(
            { 
              disbursalRequest : value
            
         }
        );

// Async/Await
const data = await 
                    customer.checkEligibility(
                    { 
                       disbursalRequest : value
                    
                     });
```





| Argument  |  Type  | Required | Description |
| --------- | -----  | -------- | ----------- |
| body | [CheckEligibilityRequest](#CheckEligibilityRequest) | yes | Request body |


Use this API to pre approve by checking the customer's credit eligibility based on  mobile number and countryCode and vintage data of monthly transactions.

*Returned Response:*




[EligibilitySuccess](#EligibilitySuccess)

Success. Returns a JSON object as shown below. Refer `EligibilitySuccess` for more details.




<details>
<summary><i>&nbsp; Examples:</i></summary>


<details>
<summary><i>&nbsp; status</i></summary>

```json
"ENABLED"
```
</details>

<details>
<summary><i>&nbsp; message</i></summary>

```json
"User is eligible to transact"
```
</details>

<details>
<summary><i>&nbsp; redirectUrl</i></summary>

```json
"https://account.potlee.co.in"
```
</details>

<details>
<summary><i>&nbsp; callbackUrl</i></summary>

```json
"https://www.google.com"
```
</details>

<details>
<summary><i>&nbsp; creditLimit</i></summary>

```json
[
  {
    "availableLimit": 300000,
    "possibleLimit": 500000,
    "lender": {
      "slug": "ugro",
      "name": "UGRO",
      "logo": "https://cdn.pixelbin.io/v2/potlee/original/public/ugro/ugro_logo"
    }
  }
]
```
</details>

</details>









---



### Schemas

 
 
 #### [UserSchema](#UserSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | firstName | string |  no  |  |
 | lastName | string |  no  |  |
 | countryCode | string |  no  |  |
 | mobile | string |  no  |  |
 | email | string |  no  |  |
 | gender | string |  no  |  |
 | dob | string |  no  |  |
 | active | boolean |  no  |  |
 | profilePicUrl | string |  no  |  |
 | isEmailVerified | boolean |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |

---


 
 
 #### [count](#count)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | totalUsers | string |  no  |  |

---


 
 
 #### [FilterByDate](#FilterByDate)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | startDate | string |  no  |  |
 | endDate | string |  no  |  |

---


 
 
 #### [LenderCount](#LenderCount)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | totalLenders | string |  no  |  |

---


 
 
 #### [LenderSchema](#LenderSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | name | string |  no  |  |
 | active | boolean |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |

---


 
 
 #### [TotalUsersPerLender](#TotalUsersPerLender)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | filters | [[Filters](#Filters)] |  yes  |  |
 | page | [PageResponse](#PageResponse) |  yes  |  |
 | lenderList | [[TotalUsersPerLenderData](#TotalUsersPerLenderData)] |  yes  |  |

---


 
 
 #### [TotalUsersPerLenderData](#TotalUsersPerLenderData)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | name | string |  no  |  |
 | active | boolean |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |
 | totalUsers | string |  no  |  |

---


 
 
 #### [TotalUserByLender](#TotalUserByLender)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  no  |  |
 | count | string |  no  |  |

---


 
 
 #### [UsersByLender](#UsersByLender)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | firstName | string |  no  |  |
 | lastName | string |  no  |  |
 | mobile | string |  no  |  |
 | email | string |  no  |  |
 | name | string |  no  |  |

---


 
 
 #### [ErrorResponse](#ErrorResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | message | string |  no  |  |
 | info | string |  no  |  |
 | code | string |  no  |  |
 | requestId | string |  no  |  |
 | meta | string |  no  |  |

---


 
 
 #### [EditProfileRequest](#EditProfileRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | firstName | string |  no  |  |
 | lastName | string |  no  |  |
 | countryCode | string |  no  |  |
 | mobile | string |  no  |  |
 | email | string |  no  |  |
 | gender | string |  no  |  |
 | dob | string |  no  |  |
 | registrationToken | string |  no  |  |

---


 
 
 #### [VerifyOtpRequest](#VerifyOtpRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | requestId | string |  yes  |  |
 | otp | string |  yes  |  |
 | captchaCode | string |  no  |  |
 | androidHash | string |  no  |  |
 | referralCode | string |  no  |  |
 | onboardingToken | string |  no  |  |

---


 
 
 #### [SendMobileOtpRequest](#SendMobileOtpRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | countryCode | string |  yes  |  |
 | mobile | string |  yes  |  |
 | captchaCode | string |  no  |  |
 | androidHash | string |  no  |  |
 | force | string |  no  |  |

---


 
 
 #### [ReSendMobileOtpRequest](#ReSendMobileOtpRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | captchaCode | string |  no  |  |
 | token | string |  yes  |  |
 | androidHash | string |  no  |  |

---


 
 
 #### [SendOtpRequest](#SendOtpRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | countryCode | string |  no  |  |
 | captchaCode | string |  no  |  |
 | mobile | string |  no  |  |

---


 
 
 #### [ApplicationUser](#ApplicationUser)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | user | [UserSchema](#UserSchema) |  no  |  |

---


 
 
 #### [SendOtpResponse](#SendOtpResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | resendTimer | number |  no  |  |
 | resendToken | string |  no  |  |
 | success | boolean |  no  |  |
 | requestId | string |  no  |  |
 | message | string |  no  |  |
 | mobile | string |  no  |  |
 | countryCode | string |  no  |  |
 | email | string |  no  |  |
 | resendEmailToken | string |  no  |  |
 | registerToken | string |  no  |  |
 | verifyEmailOtp | boolean |  no  |  |
 | verifyMobileOtp | boolean |  no  |  |
 | userExists | boolean |  no  |  |

---


 
 
 #### [EmailUpdate](#EmailUpdate)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | email | string |  no  |  |

---


 
 
 #### [UserUpdateRequest](#UserUpdateRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | firstName | any |  no  |  |
 | lastName | any |  no  |  |
 | countryCode | string |  yes  |  |
 | mobile | string |  yes  |  |
 | email | any |  no  |  |
 | gender | any |  no  |  |
 | dob | any |  no  |  |
 | active | boolean |  no  |  |
 | profilePictureUrl | any |  no  |  |
 | isEmailVerified | boolean |  no  |  |

---


 
 
 #### [LenderUpdateRequest](#LenderUpdateRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | active | boolean |  no  |  |

---


 
 
 #### [ProfileEditSuccess](#ProfileEditSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | user | [UserSchema](#UserSchema) |  no  |  |
 | registerToken | string |  no  |  |
 | resendEmailToken | string |  no  |  |
 | userExists | boolean |  no  |  |
 | verifyEmailLink | boolean |  no  |  |
 | verifyEmailOtp | boolean |  no  |  |
 | verifyMobileOtp | boolean |  no  |  |
 | email | string |  no  |  |
 | requestId | string |  no  |  |
 | countryCode | string |  no  |  |
 | mobile | string |  no  |  |
 | success | boolean |  no  |  |
 | message | string |  no  |  |
 | resendTimer | number |  no  |  |
 | resendToken | string |  no  |  |

---


 
 
 #### [LoginSuccess](#LoginSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | user | [UserSchema](#UserSchema) |  no  |  |
 | requestId | string |  no  |  |
 | registerToken | string |  no  |  |

---


 
 
 #### [VerifyOtpSuccess](#VerifyOtpSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | user | [UserSchema](#UserSchema) |  no  |  |
 | userExists | boolean |  no  |  |
 | isNew | boolean |  no  |  |

---


 
 
 #### [LogoutSuccess](#LogoutSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | logout | boolean |  no  |  |

---


 
 
 #### [OtpSuccess](#OtpSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | resendTimer | number |  no  |  |
 | resendToken | string |  no  |  |
 | registerToken | string |  no  |  |
 | success | boolean |  no  |  |
 | requestId | string |  no  |  |
 | message | string |  no  |  |
 | mobile | string |  no  |  |
 | isNew | boolean |  no  |  |
 | countryCode | string |  no  |  |
 | otpLength | number |  no  |  |

---


 
 
 #### [SessionListSuccess](#SessionListSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | sessions | [string] |  no  |  |

---


 
 
 #### [VerifyMobileOTPSuccess](#VerifyMobileOTPSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | user | [UserSchema](#UserSchema) |  no  |  |

---


 
 
 #### [Location](#Location)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | latitude | number |  no  |  |
 | longitude | number |  no  |  |

---


 
 
 #### [OrderAddress](#OrderAddress)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | line1 | string |  no  |  |
 | line2 | string |  no  |  |
 | city | string |  no  |  |
 | state | string |  no  |  |
 | country | string |  no  |  |
 | pincode | string |  no  |  |
 | type | string |  no  |  |
 | geoLocation | [Location](#Location) |  no  |  |

---


 
 
 #### [CustomerObject](#CustomerObject)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | countryCode | string |  no  |  |
 | mobile | string |  yes  |  |
 | uid | string |  yes  |  |
 | email | string |  no  |  |
 | firstname | string |  no  |  |
 | middleName | string |  no  |  |
 | lastName | string |  no  |  |

---


 
 
 #### [Order](#Order)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | valueInPaise | number |  yes  |  |
 | uid | string |  yes  |  |
 | emiTenure | number |  no  |  |
 | items | [[Items](#Items)] |  no  |  |
 | shippingAddress | [OrderAddress](#OrderAddress) |  no  |  |
 | billingAddress | [OrderAddress](#OrderAddress) |  no  |  |

---


 
 
 #### [OrderUid](#OrderUid)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | valueInPaise | number |  no  |  |
 | uid | string |  yes  |  |
 | items | [[Items](#Items)] |  no  |  |
 | shippingAddress | [OrderAddress](#OrderAddress) |  no  |  |
 | billingAddress | [OrderAddress](#OrderAddress) |  no  |  |

---


 
 
 #### [CustomerMeta](#CustomerMeta)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | ip | string |  yes  |  |
 | appVersion | string |  yes  |  |
 | appIdentifier | string |  no  |  |
 | customerUserAgent | string |  no  |  |
 | deviceId | string |  yes  |  |

---


 
 
 #### [Device](#Device)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | ipAddress | string |  yes  |  |
 | userAgent | string |  yes  |  |
 | latitude | number |  no  |  |
 | longitude | number |  no  |  |

---


 
 
 #### [VerifyCustomer](#VerifyCustomer)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | order | [Order](#Order) |  yes  |  |
 | device | [Device](#Device) |  yes  |  |
 | meta | string |  no  |  |
 | fetchLimitOptions | boolean |  no  |  |

---


 
 
 #### [CreateTransaction](#CreateTransaction)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | autoCapture | boolean |  no  |  |
 | redirectUrl | string |  yes  |  |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | order | [Order](#Order) |  yes  |  |
 | device | [Device](#Device) |  yes  |  |
 | meta | string |  no  |  |

---


 
 
 #### [ResendPaymentRequest](#ResendPaymentRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | autoCapture | boolean |  no  |  |
 | redirectUrl | string |  no  |  |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | order | [OrderUid](#OrderUid) |  yes  |  |

---


 
 
 #### [VerifyCustomerSuccess](#VerifyCustomerSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | status | string |  no  |  |
 | userStatus | string |  no  |  |
 | message | string |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [CreateTransactionSuccess](#CreateTransactionSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | chargeToken | string |  no  |  |
 | redirectUrl | string |  no  |  |
 | message | string |  yes  |  |
 | transactionId | string |  no  |  |
 | status | string |  no  |  |
 | userStatus | string |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [SupportDocuments](#SupportDocuments)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | fileName | string |  no  |  |
 | fileUrl | string |  no  |  |

---


 
 
 #### [CreateTicketResponse](#CreateTicketResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | serviceRequestId | string |  no  |  |
 | message | string |  no  |  |

---


 
 
 #### [CreateTicket](#CreateTicket)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | category | string |  yes  |  |
 | transactionId | string |  no  |  |
 | description | string |  yes  |  |
 | documents | [[SupportDocuments](#SupportDocuments)] |  no  |  |

---


 
 
 #### [InitiateTransactions](#InitiateTransactions)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [GetMobileFromToken](#GetMobileFromToken)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [GetDataFromToken](#GetDataFromToken)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [MerchantDetails](#MerchantDetails)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  no  |  |
 | website | string |  no  |  |
 | logo | string |  no  |  |

---


 
 
 #### [InitiateTransactionsSuccess](#InitiateTransactionsSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | chargeToken | string |  yes  |  |
 | session | string |  no  |  |
 | expiry | string |  no  |  |
 | hash | string |  no  |  |
 | order | [Order](#Order) |  no  |  |
 | isAsp | boolean |  no  |  |
 | merchant | [MerchantDetails](#MerchantDetails) |  no  |  |

---


 
 
 #### [RetrieveMobileFromToken](#RetrieveMobileFromToken)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | countryCode | string |  yes  |  |
 | mobile | string |  yes  |  |

---


 
 
 #### [CreateDashboardTemplateRequest](#CreateDashboardTemplateRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  yes  |  |
 | version | string |  yes  |  |
 | isDefault | boolean |  no  |  |
 | sections | [[TemplateSections](#TemplateSections)] |  yes  |  |

---


 
 
 #### [TemplateSections](#TemplateSections)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | sequence | number |  yes  |  |
 | isAvailableInMobile | boolean |  yes  |  |
 | isAvailableInDesktop | boolean |  yes  |  |
 | component | [TemplateComponent](#TemplateComponent) |  yes  |  |

---


 
 
 #### [TemplateComponent](#TemplateComponent)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  yes  |  |
 | description | string |  yes  |  |
 | isAvailableInDesktop | boolean |  no  |  |
 | partnerApplications | [[PartnerApplications](#PartnerApplications)] |  no  |  |
 | banners | [[Banners](#Banners)] |  no  |  |
 | tips | [[Tips](#Tips)] |  no  |  |

---


 
 
 #### [PartnerApplications](#PartnerApplications)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  yes  |  |
 | description | string |  no  |  |
 | urlPath | string |  no  |  |
 | urlTarget | string |  no  |  |
 | imageUrl | string |  yes  |  |
 | sequence | number |  no  |  |

---


 
 
 #### [Offerings](#Offerings)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  yes  |  |
 | description | string |  no  |  |
 | urlPath | string |  no  |  |
 | urlTarget | string |  no  |  |
 | imageUrl | string |  yes  |  |
 | sequence | number |  no  |  |
 | gradient | [string] |  yes  |  |

---


 
 
 #### [Banners](#Banners)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | imageUrl | string |  yes  |  |
 | action | [ActionSchema](#ActionSchema) |  no  |  |

---


 
 
 #### [Tips](#Tips)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  no  |  |
 | description | string |  no  |  |
 | urlPath | string |  yes  |  |
 | urlTarget | string |  no  |  |
 | imageUrl | string |  no  |  |
 | sequence | number |  no  |  |

---


 
 
 #### [DashboardTemplateResponse](#DashboardTemplateResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | name | string |  no  |  |
 | version | string |  no  |  |
 | active | boolean |  no  |  |
 | sections | [[SectionSchema](#SectionSchema)] |  yes  |  |

---


 
 
 #### [SectionSchema](#SectionSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | type | string |  yes  |  |
 | title | string |  no  |  |
 | description | string |  no  |  |
 | partners | [[PartnerApplicationsResponse](#PartnerApplicationsResponse)] |  no  |  |
 | banners | [[BannersResponse](#BannersResponse)] |  no  |  |
 | tips | [[TipsResponse](#TipsResponse)] |  no  |  |

---


 
 
 #### [PartnerApplicationsResponse](#PartnerApplicationsResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | name | string |  yes  |  |
 | description | string |  no  |  |
 | action | [ActionSchema](#ActionSchema) |  yes  |  |
 | imageUrl | string |  yes  |  |

---


 
 
 #### [OfferingsResponse](#OfferingsResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | name | string |  yes  |  |
 | description | string |  no  |  |
 | action | [ActionSchema](#ActionSchema) |  yes  |  |
 | imageUrl | string |  yes  |  |
 | gradient | [string] |  yes  |  |

---


 
 
 #### [BannersResponse](#BannersResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | action | [ActionSchema](#ActionSchema) |  no  |  |
 | imageUrl | string |  yes  |  |

---


 
 
 #### [TipsSection](#TipsSection)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | tips | [[TipsResponse](#TipsResponse)] |  no  |  |
 | categories | [[TipsCategories](#TipsCategories)] |  no  |  |
 | action | [ActionSchema](#ActionSchema) |  no  |  |

---


 
 
 #### [TipsResponse](#TipsResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  no  |  |
 | category | string |  no  |  |
 | description | string |  no  |  |
 | action | [ActionSchema](#ActionSchema) |  yes  |  |
 | imageUrl | string |  no  |  |

---


 
 
 #### [TipsCategories](#TipsCategories)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | title | string |  yes  |  |

---


 
 
 #### [ActionSchema](#ActionSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | type | string |  no  |  |
 | page | [PageSchema](#PageSchema) |  no  |  |
 | popup | [PageSchema](#PageSchema) |  no  |  |

---


 
 
 #### [UpdateDashboardTemplateRequest](#UpdateDashboardTemplateRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | version | string |  no  |  |
 | isDefault | boolean |  no  |  |
 | active | boolean |  no  |  |
 | sections | [[UpdateTemplateSections](#UpdateTemplateSections)] |  no  |  |

---


 
 
 #### [UpdateTemplateSections](#UpdateTemplateSections)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | sequence | number |  no  |  |
 | isAvailableInMobile | boolean |  no  |  |
 | isAvailableInDesktop | boolean |  no  |  |
 | active | boolean |  no  |  |
 | component | [UpdateTemplateComponent](#UpdateTemplateComponent) |  no  |  |

---


 
 
 #### [UpdateTemplateComponent](#UpdateTemplateComponent)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | description | string |  no  |  |
 | isAvailableInDesktop | boolean |  no  |  |
 | active | boolean |  no  |  |
 | partners | [[UpdatePartnerApplications](#UpdatePartnerApplications)] |  no  |  |
 | banners | [[UpdateBanners](#UpdateBanners)] |  no  |  |
 | tips | [[UpdateTips](#UpdateTips)] |  no  |  |

---


 
 
 #### [UpdatePartnerApplications](#UpdatePartnerApplications)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | description | string |  no  |  |
 | action | string |  no  |  |
 | imageUrl | string |  no  |  |
 | sequence | number |  no  |  |
 | active | boolean |  no  |  |

---


 
 
 #### [UpdateOfferings](#UpdateOfferings)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | description | string |  no  |  |
 | urlPath | string |  no  |  |
 | urlTarget | string |  no  |  |
 | imageUrl | string |  no  |  |
 | sequence | number |  no  |  |
 | gradient | [string] |  no  |  |

---


 
 
 #### [UpdateBanners](#UpdateBanners)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | imageUrl | string |  no  |  |
 | action | string |  no  |  |
 | sequence | number |  no  |  |
 | active | boolean |  no  |  |

---


 
 
 #### [UpdateTips](#UpdateTips)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |
 | name | string |  no  |  |
 | description | string |  no  |  |
 | imageUrl | string |  no  |  |
 | action | string |  no  |  |
 | sequence | number |  no  |  |
 | active | boolean |  no  |  |

---


 
 
 #### [NavigationsMobileResponse](#NavigationsMobileResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | tabs | [[TabsSchema](#TabsSchema)] |  yes  |  |
 | profileSections | [[ProfileSectionSchema](#ProfileSectionSchema)] |  yes  |  |

---


 
 
 #### [TabsSchema](#TabsSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | title | string |  yes  |  |
 | page | [PageSchema](#PageSchema) |  yes  |  |
 | icon | string |  yes  |  |
 | activeIcon | string |  yes  |  |
 | active | boolean |  yes  |  |

---


 
 
 #### [PageSchema](#PageSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | link | string |  no  |  |
 | type | [PageType](#PageType) |  no  |  |
 | params | [String: [string]] |  no  |  |
 | query | [String: string] |  no  |  |

---


 
 
 #### [ProfileSectionSchema](#ProfileSectionSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | title | string |  yes  |  |
 | navigations | [[ProfileNavigationSchema](#ProfileNavigationSchema)] |  yes  |  |
 | active | boolean |  yes  |  |

---


 
 
 #### [ProfileNavigationSchema](#ProfileNavigationSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | title | string |  yes  |  |
 | description | string |  no  |  |
 | icon | string |  yes  |  |
 | type | string |  yes  |  |
 | action | [ActionSchema](#ActionSchema) |  no  |  |
 | active | boolean |  no  |  |

---


 
 
 #### [SendPNSRegisterRequest](#SendPNSRegisterRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | deviceId | string |  yes  |  |
 | deviceType | string |  yes  |  |
 | token | string |  yes  |  |

---


 
 
 #### [PNSRegisterResponse](#PNSRegisterResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | status | boolean |  no  |  |
 | message | string |  no  |  |

---


 
 
 #### [FaqResponse](#FaqResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | categories | [[CategorySchema](#CategorySchema)] |  no  |  |

---


 
 
 #### [CategorySchema](#CategorySchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | uid | string |  yes  |  |
 | title | string |  no  |  |
 | description | string |  no  |  |
 | logo | string |  no  |  |
 | questions | [[QuestionSchema](#QuestionSchema)] |  no  |  |

---


 
 
 #### [QuestionSchema](#QuestionSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | uid | string |  yes  |  |
 | title | string |  no  |  |
 | description | string |  no  |  |
 | displayOrder | number |  no  |  |
 | canRaiseRequest | boolean |  no  |  |

---


 
 
 #### [SupportCategories](#SupportCategories)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | kind | string |  no  |  |
 | display | string |  no  |  |

---


 
 
 #### [SupportCategoriesResponse](#SupportCategoriesResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | categories | [[SupportCategories](#SupportCategories)] |  no  |  |

---


 
 
 #### [SanctionLetterResponse](#SanctionLetterResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | sanctionedLetterFileUrl | string |  yes  |  |

---


 
 
 #### [KfsDocumentResponse](#KfsDocumentResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | kfsFileUrl | string |  yes  |  |

---


 
 
 #### [UserWhiteListedResponse](#UserWhiteListedResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | status | string |  no  |  |

---


 
 
 #### [UserConsentRequest](#UserConsentRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | consents | [string] |  no  |  |

---


 
 
 #### [Consents](#Consents)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | type | string |  no  |  |
 | text | string |  no  |  |

---


 
 
 #### [UserConsentRequestV2](#UserConsentRequestV2)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | consents | [[Consents](#Consents)] |  no  |  |

---


 
 
 #### [UserConsentResponse](#UserConsentResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | success | boolean |  no  |  |

---


 
 
 #### [UserKycSteps](#UserKycSteps)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | index | string |  no  |  |
 | name | string |  no  |  |
 | rules | string |  no  |  |
 | active | boolean |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |

---


 
 
 #### [CreateKycStepRequest](#CreateKycStepRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  yes  |  |
 | index | string |  yes  |  |
 | active | boolean |  yes  |  |
 | rules | string |  no  |  |

---


 
 
 #### [RemoveKycStepRequest](#RemoveKycStepRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | name | string |  no  |  |
 | index | string |  yes  |  |
 | active | boolean |  no  |  |
 | rules | string |  no  |  |

---


 
 
 #### [KycUpdateMessage](#KycUpdateMessage)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | message | string |  no  |  |

---


 
 
 #### [MobileFromLinkingRequest](#MobileFromLinkingRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [MobileFromLinkingResponse](#MobileFromLinkingResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | countryCode | string |  yes  |  |
 | mobile | string |  yes  |  |

---


 
 
 #### [SessionFromLinkingRequest](#SessionFromLinkingRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [SessionFromLinkingResponse](#SessionFromLinkingResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | session | string |  yes  |  |
 | expiry | number |  yes  |  |

---


 
 
 #### [LinkAccount](#LinkAccount)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | redirectUrl | string |  yes  |  |
 | device | [Device](#Device) |  yes  |  |

---


 
 
 #### [LinkAccountSuccess](#LinkAccountSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | redirectUrl | string |  no  |  |
 | statusCode | number |  no  |  |
 | status | string |  no  |  |
 | message | string |  no  |  |
 | errorCode | string |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [UnlinkAccount](#UnlinkAccount)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | device | [Device](#Device) |  yes  |  |

---


 
 
 #### [UnlinkAccountSuccess](#UnlinkAccountSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | status | string |  yes  |  |
 | message | string |  yes  |  |
 | statusCode | number |  yes  |  |
 | userStatus | string |  no  |  |
 | errorCode | string |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [Refund](#Refund)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | fingerprint | string |  no  |  |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | refundItems | [[Items](#Items)] |  no  |  |
 | orderId | string |  yes  |  |
 | refundId | string |  yes  |  |
 | refundAmount | number |  yes  |  |

---


 
 
 #### [Translation](#Translation)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | content | any |  no  |  |

---


 
 
 #### [FilterKeys](#FilterKeys)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | display | string |  no  |  |
 | name | string |  no  |  |
 | kind | string |  no  |  |

---


 
 
 #### [FilterValues](#FilterValues)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | display | string |  no  |  |
 | isSelected | boolean |  no  |  |
 | value | string |  no  |  |

---


 
 
 #### [Filters](#Filters)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | key | [FilterKeys](#FilterKeys) |  no  |  |
 | values | [[FilterValues](#FilterValues)] |  no  |  |

---


 
 
 #### [PageResponse](#PageResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | type | string |  yes  |  |
 | current | number |  yes  |  |
 | hasPrevious | boolean |  yes  |  |
 | hasNext | boolean |  yes  |  |
 | size | number |  yes  |  |
 | itemTotal | number |  yes  |  |

---


 
 
 #### [UserResponse](#UserResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | filters | [[Filters](#Filters)] |  yes  |  |
 | page | [PageResponse](#PageResponse) |  yes  |  |
 | listOfUsers | [[UserSchema](#UserSchema)] |  yes  |  |

---


 
 
 #### [UserDetailRequest](#UserDetailRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  yes  |  |

---


 
 
 #### [UserConsents](#UserConsents)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | userId | string |  no  |  |
 | ipAddress | string |  no  |  |
 | text | string |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |

---


 
 
 #### [CreditScoreSchema](#CreditScoreSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | userId | string |  no  |  |
 | cibil | number |  no  |  |
 | finbox | string |  no  |  |
 | systemAwarded | string |  no  |  |
 | isActive | boolean |  no  |  |
 | deletedAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | createdAt | string |  no  |  |

---


 
 
 #### [CreditLimitSchema](#CreditLimitSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | userId | string |  no  |  |
 | creditLimit | string |  no  |  |
 | createdAt | string |  no  |  |
 | updatedAt | string |  no  |  |
 | deletedAt | string |  no  |  |

---


 
 
 #### [Screen](#Screen)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | screenType | string |  no  |  |
 | name | string |  no  |  |
 | link | string |  no  |  |

---


 
 
 #### [UserStateSchema](#UserStateSchema)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | screen | [Screen](#Screen) |  no  |  |

---


 
 
 #### [GetAccessTokenResponse](#GetAccessTokenResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | success | boolean |  no  |  |
 | accessToken | string |  no  |  |
 | refreshToken | string |  no  |  |
 | tokenExpireAt | string |  no  |  |
 | tokenExpiryIn | string |  no  |  |
 | refreshTokenExpiryAt | string |  no  |  |
 | refreshTokenExpiryIn | string |  no  |  |
 | scope | [string] |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [RefreshTokenResponse](#RefreshTokenResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | success | boolean |  no  |  |
 | accessToken | string |  no  |  |
 | tokenExpireAt | string |  no  |  |
 | tokenExpiryIn | string |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [RefreshTokenRequest](#RefreshTokenRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | token | string |  yes  |  |

---


 
 
 #### [Items](#Items)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | category | string |  no  |  |
 | sku | string |  no  |  |
 | rate | number |  no  |  |
 | quantity | number |  no  |  |

---


 
 
 #### [RefundStatusList](#RefundStatusList)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | id | string |  no  |  |
 | orderItems | [[Items](#Items)] |  no  |  |
 | amount | number |  no  |  |
 | status | string |  no  |  |
 | createdAt | string |  no  |  |
 | processedDate | string |  no  |  |

---


 
 
 #### [RefundStatus](#RefundStatus)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | orderId | string |  no  |  |
 | userId | string |  no  |  |
 | merchantId | string |  no  |  |
 | lenderId | string |  no  |  |
 | loanAccountNumber | string |  no  |  |
 | refund | [[RefundStatusList](#RefundStatusList)] |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [CustomerMetricsPivots](#CustomerMetricsPivots)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | date | string |  no  |  |
 | sum | number |  no  |  |

---


 
 
 #### [CustomerMetricsSubResponse](#CustomerMetricsSubResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | total | string |  no  |  |
 | pivots | [[CustomerMetricsPivots](#CustomerMetricsPivots)] |  no  |  |
 | title | string |  no  |  |
 | description | string |  no  |  |
 | valueFormat | string |  no  |  |
 | logo | string |  no  |  |

---


 
 
 #### [CustomerMetricsAnalytics](#CustomerMetricsAnalytics)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | totalCustomers | [CustomerMetricsSubResponse](#CustomerMetricsSubResponse) |  no  |  |
 | source | [CustomerMetricsSubResponse](#CustomerMetricsSubResponse) |  no  |  |

---


 
 
 #### [CustomerMetricsFilters](#CustomerMetricsFilters)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | type | string |  yes  |  |
 | display | string |  yes  |  |
 | value | [string] |  yes  |  |
 | isSelected | boolean |  no  |  |
 | isActive | boolean |  yes  |  |

---


 
 
 #### [CustomerMetrics](#CustomerMetrics)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | metrics | [CustomerMetricsAnalytics](#CustomerMetricsAnalytics) |  no  |  |
 | filters | [[CustomerMetricsFilters](#CustomerMetricsFilters)] |  no  |  |
 | sort | [[CustomerMetricsFilters](#CustomerMetricsFilters)] |  no  |  |

---


 
 
 #### [CustomerMetricsResponse](#CustomerMetricsResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | data | [CustomerMetrics](#CustomerMetrics) |  no  |  |

---


 
 
 #### [CustomerMetricsRequest](#CustomerMetricsRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | filters | [[CustomerMetricsFilters](#CustomerMetricsFilters)] |  no  |  |
 | sort | [[CustomerMetricsFilters](#CustomerMetricsFilters)] |  no  |  |
 | merchantId | string |  no  |  |
 | lenderId | string |  no  |  |
 | pivotPoints | number |  no  |  |

---


 
 
 #### [SourceAnalyticsRequest](#SourceAnalyticsRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | filters | [[CustomerMetricsFilters](#CustomerMetricsFilters)] |  no  |  |

---


 
 
 #### [LenderResponse](#LenderResponse)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | slug | string |  no  |  |
 | name | string |  no  |  |
 | logo | string |  no  |  |

---


 
 
 #### [CreditLimitObject](#CreditLimitObject)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | availableLimit | number |  no  |  |
 | possibleLimit | number |  no  |  |
 | lender | [LenderResponse](#LenderResponse) |  no  |  |

---


 
 
 #### [BusinessDetails](#BusinessDetails)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | category | string |  yes  |  |
 | shopName | string |  no  |  |
 | legalName | string |  yes  |  |
 | address | string |  no  |  |
 | type | string |  no  |  |
 | pincode | string |  no  |  |

---


 
 
 #### [DocumentItems](#DocumentItems)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | number | string |  no  |  |
 | category | string |  no  |  |
 | type | string |  no  |  |
 | name | string |  no  |  |
 | issuedOn | string |  no  |  |
 | issuedAt | string |  no  |  |
 | issuedBy | string |  no  |  |
 | expiryOn | string |  no  |  |

---


 
 
 #### [VintageItems](#VintageItems)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | month | number |  yes  |  |
 | year | number |  yes  |  |
 | totalTransactions | number |  yes  |  |
 | totalTransactionAmount | number |  yes  |  |
 | totalCancellations | number |  no  |  |
 | totalCancellationAmount | number |  no  |  |

---


 
 
 #### [EligibilitySuccess](#EligibilitySuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | status | string |  no  |  |
 | message | string |  no  |  |
 | redirectUrl | string |  no  |  |
 | callbackUrl | string |  no  |  |
 | creditLimits | [[CreditLimitObject](#CreditLimitObject)] |  no  |  |
 | __headers | string |  no  |  |

---


 
 
 #### [CheckEligibilityRequest](#CheckEligibilityRequest)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | customer | [CustomerObject](#CustomerObject) |  yes  |  |
 | order | [Order](#Order) |  no  |  |
 | businessDetails | [BusinessDetails](#BusinessDetails) |  no  |  |
 | documents | [[DocumentItems](#DocumentItems)] |  no  |  |
 | device | [Device](#Device) |  yes  |  |
 | vintage | [[VintageItems](#VintageItems)] |  no  |  |
 | meta | string |  no  |  |
 | fetchLimitOptions | boolean |  no  |  |

---


 
 
 #### [GetSchemesSuccess](#GetSchemesSuccess)

 | Properties | Type | Nullable | Description |
 | ---------- | ---- | -------- | ----------- |
 | userId | string |  no  |  |
 | lenders | [undefined] |  yes  |  |
 | __headers | string |  no  |  |

---




### Enums





 #### [PageType](#PageType)
 Type : string

 | Name | Value | Description |
 | ---- | ----- | ----------- |
 | external | external | Symbolic link for External Link: /external/:url |
 | login | login | Symbolic link for Login: /login |
 | home | home | Symbolic link for Home: / |
 | transactions | transactions | Symbolic link for Transactions: /transactions |
 | transactionDetails | transactionDetails | Symbolic link for Transaction Details: /transactions/:id |
 | rewards | rewards | Symbolic link for Rewards: /rewards |
 | referAndEarn | referAndEarn | Symbolic link for Refer: /refer |
 | profile | profile | Symbolic link for Profile: /profile |
 | setupAutopay | setupAutopay | Symbolic link for AutoPay: /autopay |
 | updateEmail | updateEmail | Symbolic link for Update Email: /profile/email |
 | reportIssue | reportIssue | Symbolic link for Report Issue: /profile/report |
 | creditScore | creditScore | Symbolic link for Credit Score: /credit-score |
 | autoPay | autoPay | Symbolic link for Setup Autopay: /autopay |
 | helpCenter | helpCenter | Symbolic link for Help Center: /profile/help-center |
 | kycInit | kycInit | Symbolic link for Start KYC: /kyc |
 | accessDigilocker | accessDigilocker | Symbolic link for Access Digilocker: /kyc/:lender/access-digilocker |
 | liveliness | liveliness | Symbolic link for Liveliness: /kyc/:lender/selfie |
 | lenderOnboard | lenderOnboard | Symbolic link for Lender Onboard: /kyc/:lender/lender-onboard |
 | lender | lender | Symbolic link for Lender: /lender/:lenderName |
 | kycDocs | kycDocs | Symbolic link for Verify KYC Documents: /kyc/documents |
 | kycSelfie | kycSelfie | Symbolic link for Verify KYC Selfie: /kyc/selfie |
 | kycStatus | kycStatus | Symbolic link for KYC Status: /kyc/status |
 | kycError | kycError | Symbolic link for KYC Error: /kyc/error |
 | kycDigilockerResponse | kycDigilockerResponse | Symbolic link for KYC Digilocker Response: /kyc/digilocker-response |
 | kycInitResponse | kycInitResponse | Symbolic link for KYC Init Response: /kyc/init-response |
 | repayment | repayment | Symbolic link for Repayment: /repayment |
 | netBankingRepayment | netBankingRepayment | Symbolic link for Net Banking Repayment: /repayment/netbanking |
 | upiRepayment | upiRepayment | Symbolic link for UPI Repayment: /repayment/upi |
 | sanctionLetter | sanctionLetter | Symbolic link for Sanction Letter: /sanction/:userId |
 | kfs | kfs | Symbolic link for KFS: /kfs/:userId |

---






