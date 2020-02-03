1-1. OCPインストール前の準備  

 1. ssh で環境にログインします。  
    ※ AWS のアカウント情報は環境払い出した後に受信するメールに記載されておりますのでそちらでご確認ください。    
 2. sudo コマンドで root 権限を取得します  
    sudo -i  
    echo ${GUID}  
    Install the AWS CLI tools:  
    
    $ GUID=yourname
    $ oc new-project pipeline-${GUID}-dev --description="Cat of the Day Development Environment" --display-name="Cat Of The Day - Dev"
 


