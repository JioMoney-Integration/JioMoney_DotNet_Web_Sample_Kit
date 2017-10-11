# JioMoney_DotNet_Web_Sample_Kit
This is JioMoney’s DotNet based sample library for integration of redirection based Payment Gateway/ Wallet</br>
# Installation :
<pre><b>• STEP1:</b> Download the JioMoney_IntLibrary.dll from the integration kit.
  
<b>• STEP2:</b> Open the Merchant Website in Solution Explorer.
  
<b>• STEP3:</b> Navigate to the References part, Right Click and click on Add Reference.
  
<b>• STEP4:</b> Browse the Location and select the JioMoney_IntLibrary.dll and click ok.
  
<b>• STEP5:</b> Add using JioMoney_IntLibrary; on top in the code behind.

<b>• STEP6:</b> Call the respective method mentioned above and pass the parameters as shown below.

JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMPaymentAPI(merchantid, clientid, channel, returl, checksum, token, transaction_extref,transaction_timestamp, transaction_txntype, transaction_amount, transaction_currency,subscriber_customerid, subscriber_customername, subscriber_mobilenumber, udf1, udf2,udf3, udf4, udf5, productdescription, version, apiurl);

<b>• STEP7:</b> For payment API response will be received on the return url passed above in returl

</br></pre>

# Initiating payment request :</br>

<pre> JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMPaymentAPI(merchantid, clientid, channel, returl, checksum, token, transaction_extref, transaction_timestamp, transaction_txntype, transaction_amount, transaction_currency, subscriber_customerid, subscriber_customername, subscriber_mobilenumber, udf1, udf2, udf3, udf4, udf5, productdescription, version, apiurl);</br></pre> 
                  
# Initiating refund request : </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMRefundAPI(merchant_id, checksum, txn_amount, tran_ref_no, timestamp, org_jm_tran_ref_no, org_txn_timestamp, additional_info, mobile_no, version, apiurl);</pre>

# Check payment status - CHECKPAYMENTSTATUS: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMCheckPaymentStatusAPI(merchant_id, checksum, request_id, timestamp, tran_ref_no, org_txn_timestamp, version, apiurl);</pre>

# Check refund status - GETREQUESTSTATUS: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMGetRequestStatusAPI(merchant_id, checksum, mode, "NA", "NA", request_id, timestamp, tran_ref_no, org_txn_timestamp, version, apiurl);</pre>

# Check MDR - GETMDR: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMGetMDRAPI(merchant_id, checksum, mode, "NA", "NA", request_id, timestamp, tran_ref_no, org_txn_timestamp, version, apiurl);</pre>

# Check transaction details - GETTRANSACTIONDETAILS: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMGetTransactionDetailsAPI(merchant_id, checksum, mode, StartDateTime, EndDateTime, request_id, timestamp, tran_ref_no, org_txn_timestamp, version, apiurl);</pre>

# Fetch transaction period - FETCHTRANSACTIONPERIOD: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMFetchTransactionPeriodAPI(merchant_id, checksum, mode, StartDateTime, EndDateTime, request_id, timestamp, tran_ref_no, org_txn_timestamp, version, apiurl);</pre>

# Check transaction status - STATUSQUERY: </br>
<pre>JioMoney_IntLibrary.JioMoney_APILibrary.Call_JMStatusQueryAPI(clientid, merchant_id, checksum, tran_ref_no, version, apiurl);</pre>
