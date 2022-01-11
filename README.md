# Drupal 9 Starter FrameWork

## Configuration Management
We use [config split module](https://www.drupal.org/project/config_split) to manage the config files.
Some configuration are specific to the environement

### Development environement
To enables modules such as Devel, Add this line of code to `setttings.local.php`
```
$config['config_split.config_split.dev']['status'] = TRUE;
```

### Production environment
```
$config['config_split.config_split.live']['status'] = TRUE;
```