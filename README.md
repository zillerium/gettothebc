This is the hackathon repo. This is being held at Oracle in London.

The challenge is the Open one.

READ THE CONTRACT DETAILS

curl -i -X GET -u gettotheblockchain:8q6VU2Oav https://E0BBA3A3145845FAA4BCC18391B1FA6C.blockchain.ocp.oraclecloud.com:443/console/admin/api/v1.1/chaincodes/sample10

EXECUTE THE CONTRACT

curl -i --header "Content-Type: application/json"   -X POST -u gettotheblockchain:8q6VU2Oav -d  '{ "channel": "gettothebc", "chaincode": "sample10", "method": "invoke", "chaincodeVer": "v1", "args": ["a", "b", "2"], "proposalWaitTime": 50000, "transactionWaitTime": 60000 }' https://E0BBA3A3145845FAA4BCC18391B1FA6C.blockchain.ocp.oraclecloud.com:443/restproxy1/bcsgw/rest/v1/transaction/invocation
