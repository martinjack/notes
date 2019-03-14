# Permission folders
### Set current user owner folder
```
sudo chown -R $USER:www-data laravel_project
```
### Set permission 664 folders
```
sudo find laravel_project type d -exec chmod 664 {} \;
```
### Set permission 775 files
```
sudo find laravel_project type f -exec chmod 775 {} \;
```