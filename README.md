# HistoryDocs

##武林传说
Login Sequence

Client->FLServer:stUserVerifyVerCmd
Client->FLServer:stUserRequestLoginCmd
FLServer->SuperServer:t_NewSession_Session
SuperServer->BillServer:t_NewSession_Bill
BillServer->GatewayServer:t_NewSession_Gateway
FLServer-->Client:stServerReturnLoginSuccessCmd
Client->GatewayServer:Cmd::stUserVerifyVerCmd
Client->GatewayServer:Cmd::stPasswdLogonUserCmd
Client->GatewayServer:[开始游戏业务逻辑]
![image](https://github.com/wangchong-fly123/HistoryDocs/raw/master/wulin_login.jpg)
