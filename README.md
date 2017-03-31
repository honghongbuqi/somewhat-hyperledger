# somewhat-hyperledger
折腾三天终于完成了1.0开发环境的部署， 能测试chaincode了好开心啊

待解决问题：

在执行 create channel 或 join channel 时

CORE_PEER_COMMITTER_LEDGER_ORDERER=orderer:7050 peer channel create -c myc1 

CORE_PEER_ADDRESS=peer0:7051 peer channel join -b myc1.block 

有时会报错 Error: Error getting broadcast client: Error connecting to orderer:7050 due to grpc: timed out when dialing

多次重复执行可通过该操作
