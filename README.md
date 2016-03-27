# HistoryDocs

##武林传说
Login Sequence

<p>Client->FLServer:stUserVerifyVerCmd
<p>Client->FLServer:stUserRequestLoginCmd
<p>FLServer->SuperServer:t_NewSession_Session
<p>SuperServer->BillServer:t_NewSession_Bill
<p>BillServer->GatewayServer:t_NewSession_Gateway
<p>FLServer-->Client:stServerReturnLoginSuccessCmd
<p>Client->GatewayServer:Cmd::stUserVerifyVerCmd
<p>Client->GatewayServer:Cmd::stPasswdLogonUserCmd
<p>Client->GatewayServer:[开始游戏业务逻辑]
![image](https://github.com/wangchong-fly123/HistoryDocs/raw/master/wulin_login.jpg)
