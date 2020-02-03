1-1. OCPインストール前の準備  

 1. ssh で環境にログインします。  
    ※ AWS のアカウント情報は環境払い出した後に受信するメールでご確認ください。
 2. sudo コマンドを利用して root 権限を取得します。  
`   sudo -i  
    echo ${GUID}`  

 3. AWS の CLI ツールをインストールします。  
`   AWS コマンドラインインターフェースのダウンロード  
    curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"  
    unzip awscli-bundle.zip`  
  
    AWS CLI のインストール  
    ./awscli-bundle/install -i /usr/local/aws -b /bin/aws  

    AWS CLI の動作確認  
    aws --version  

    ダウンロードファイルの削除
    rm -rf /root/awscli-bundle /root/awscli-bundle.zip `
    
aa

 
 
 aa




 2.sudo コマンドを利用して root 権限を取得します。  
