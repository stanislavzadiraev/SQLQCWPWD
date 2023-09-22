# SQLQCWPWD
SQL Queries to Change WordPress Website Domain Name
```
UPDATE wp_options SET option_value = REPLACE(option_value, 'OLDDOMAINNAME', 'NEWDOMAINNAME');

UPDATE wp_users SET user_url = REPLACE (user_url, 'OLDDOMAINNAME','NEWDOMAINNAME');
UPDATE wp_usermeta SET meta_value = REPLACE (meta_value, 'OLDDOMAINNAME','NEWDOMAINNAME');

UPDATE wp_posts SET guid = REPLACE (guid, 'OLDDOMAINNAME', 'NEWDOMAINNAME');
UPDATE wp_posts SET post_content = REPLACE (post_content, 'OLDDOMAINNAME', 'NEWDOMAINNAME');
UPDATE wp_posts SET post_excerpt = REPLACE (post_excerpt, 'OLDDOMAINNAME', 'NEWDOMAINNAME');
UPDATE wp_postmeta SET meta_value = REPLACE (meta_value, 'OLDDOMAINNAME','NEWDOMAINNAME');


UPDATE wp_comments SET comment_author_url = REPLACE (comment_author_url, 'OLDDOMAINNAME','NEWDOMAINNAME');

UPDATE wp_wc_admin_notes SET image = REPLACE (image, 'OLDDOMAINNAME','NEWDOMAINNAME');
UPDATE wp_wc_admin_note_actions SET query = REPLACE (query, 'OLDDOMAINNAME','NEWDOMAINNAME');

UPDATE wp_wc_product_download_directories SET url = REPLACE (url, 'OLDDOMAINNAME','NEWDOMAINNAME');
```
and reverce
```
UPDATE wp_options SET option_value = REPLACE(option_value, 'NEWDOMAINNAME', 'OLDDOMAINNAME');

UPDATE wp_users SET user_url = REPLACE (user_url, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
UPDATE wp_usermeta SET meta_value = REPLACE (meta_value, 'NEWDOMAINNAME', 'OLDDOMAINNAME');

UPDATE wp_posts SET guid = REPLACE (guid, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
UPDATE wp_posts SET post_content = REPLACE (post_content, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
UPDATE wp_posts SET post_excerpt = REPLACE (post_excerpt, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
UPDATE wp_postmeta SET meta_value = REPLACE (meta_value, 'NEWDOMAINNAME', 'OLDDOMAINNAME');


UPDATE wp_comments SET comment_author_url = REPLACE (comment_author_url, 'NEWDOMAINNAME', 'OLDDOMAINNAME');

UPDATE wp_wc_admin_notes SET image = REPLACE (image, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
UPDATE wp_wc_admin_note_actions SET query = REPLACE (query, 'NEWDOMAINNAME', 'OLDDOMAINNAME');

UPDATE wp_wc_product_download_directories SET url = REPLACE (url, 'NEWDOMAINNAME', 'OLDDOMAINNAME');
```