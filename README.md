# docker-compose-gitlab
Docker compose for Gitlab.

Email notification config:
```
gitlab_rails['gitlab_email_enabled'] = true
gitlab_rails['gitlab_email_from'] = 'EMAIL_ADDRESS'
gitlab_rails['gitlab_email_reply_to'] = 'EMAIL_ADDRESS'
gitlab_rails['gitlab_email_display_name'] = 'Git SCM'
gitlab_rails['gitlab_email_subject_suffix'] = ''

gitlab_rails['smtp_enable'] = true
gitlab_rails['smtp_address'] = "smtpdm.aliyun.com"
gitlab_rails['smtp_port'] = 465
gitlab_rails['smtp_user_name'] = "EMAIL_ADDRESS"
gitlab_rails['smtp_password'] = "GC6Yi873tUqytY5"
gitlab_rails['smtp_domain'] = "smtpdm.aliyun.com"
gitlab_rails['smtp_authentication'] = "login"
gitlab_rails['smtp_enable_starttls_auto'] = true
gitlab_rails['smtp_tls'] = true
```

Login with username `root` and the password form the following command:
```sh
docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password
```
