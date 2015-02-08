ansible-webapp-complete
=======


    cd ansible
    ansible-playbook -i development site.yml [-t tagnames]


### Environment
* nodejs
* nginx
* mariadb
* redis
* supervisord

#### Options
* user
* user_name
* repo
  * アプリケーション本体。cloneしたものを `{{app_base_directory}}` に展開する
* app_base_directory
  * supervisordでこの直下の `app.js` が起動対象になる。
* conf_directory
  * `nginx.conf` などのconfigファイルが格納されているパス。cloneするリポジトリ内に含まれている想定
