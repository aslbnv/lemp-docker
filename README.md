launch.json for xdebug
```json
"name": "Listen for Xdebug",
            "type": "php",
            "request": "launch",
            "port": 9003,
            "hostname": "0.0.0.0",
            "pathMappings": {
                "/var/www/html": "${workspaceFolder}/src"
            }
```