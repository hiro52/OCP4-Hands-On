1-1. OCPインストール前の準備  

 1. ssh で環境にログインします。  
    ※ AWS のアカウント情報は環境払い出した後に受信するメールでご確認ください。
 2. sudo コマンドを利用して root 権限を取得します。 
```
sudo -i  
echo ${GUID}
```

 3. AWS の CLI ツールをインストールします。  
```
#AWS コマンドラインインターフェースのダウンロード  
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"  
unzip awscli-bundle.zip`  
  
#AWS CLI のインストール  
./awscli-bundle/install -i /usr/local/aws -b /bin/aws  

#AWS CLI の動作確認  
aws --version  

#ダウンロードファイルの削除  
rm -rf /root/awscli-bundle /root/awscli-bundle.zip  
```
※ OpenShift インストーラーにはこれらのツールは必要ありませんが、後で使用して資格情報を確認し、作成されたAWSリソースを一覧表示します。

 4. OpenShift のインストールバイナリをダウンロードします。 
```
OCP_VERSION=4.1.0
wget https://mirror.openshift.com/pub/openshift-v4/clients/ocp/${OCP_VERSION}/openshift-install-linux-${OCP_VERSION}.tar.gz
tar zxvf openshift-install-linux-${OCP_VERSION}.tar.gz -C /usr/bin
rm -f openshift-install-linux-${OCP_VERSION}.tar.gz /usr/bin/README.md
chmod +x /usr/bin/openshift-install
```

aa

 
 
 aa




 2.sudo コマンドを利用して root 権限を取得します。  
