# SQLQCWPWD
SQL Queries to Change WordPress Website Domain Name
```
UPDATE wp_options SET option_value = REPLACE(option_value, 'OLD.DOMAIN.NAME', 'NEW.DOMAIN.NAME');

UPDATE wp_users SET user_url = REPLACE (user_url, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');
UPDATE wp_usermeta SET meta_value = REPLACE (meta_value, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');

UPDATE wp_posts SET guid = REPLACE (guid, 'OLD.DOMAIN.NAME', 'NEW.DOMAIN.NAME');
UPDATE wp_posts SET post_content = REPLACE (post_content, 'OLD.DOMAIN.NAME', 'NEW.DOMAIN.NAME');
UPDATE wp_posts SET post_excerpt = REPLACE (post_excerpt, 'OLD.DOMAIN.NAME', 'NEW.DOMAIN.NAME');
UPDATE wp_postmeta SET meta_value = REPLACE (meta_value, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');


UPDATE wp_comments SET comment_author_url = REPLACE (comment_author_url, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');

UPDATE wp_wc_admin_notes SET image = REPLACE (image, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');
UPDATE wp_wc_admin_note_actions SET query = REPLACE (query, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');

UPDATE wp_wc_product_download_directories SET url = REPLACE (url, 'OLD.DOMAIN.NAME','NEW.DOMAIN.NAME');
```
