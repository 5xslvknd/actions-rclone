# Actions_rclone

使用 gclone 实现多网盘备份

# Secrets 

| 名称                      |          内容           |
| ------------------------ | ----------------------- |
| `RCLONE_CONFIG`          |   Rclone 配置                   |
| `GCLONE_CONFIG`          |   Gclone 配置                   |
| `GCLONE_SA_DLURL`        |   service_account 文件下载地址   |
| `GCLONE_PATCH`           |   同步目录                      |

## GCLONE_CONFIG 变量说明

使用 rclone 生成配置文件

```

[A]
type = drive
client_id = XXX
client_secret = XXX
scope = drive
token = {"access_token":"XXX","token_type":"Bearer","refresh_token":"XXX","expiry":"XXX"}

[B]
type = drive
client_id = XXX
client_secret = XXX
scope = drive
token = {"access_token":"XXX","token_type":"Bearer","refresh_token":"XXX","expiry":"XXX"}

```

## GCLONE_SA_DLURL 变量说明

service_account 文件压缩包的直链下载地址，建议上传到 dropbox 后生成下载地址

## GCLONE_PATCH 变量说明

同步目录 `source:sourcepath dest:destpath`

```

A:{folde_id1} B:{folde_id2}

```


# 鸣谢

[@rclone](https://github.com/rclone/rclone)

[@xyou365](https://github.com/xyou365/AutoRclone)

[@donwa](https://github.com/donwa/gclone)

[@wekingchen](https://github.com/wekingchen/Rclone-Actions)

[@artxia](https://github.com/artxia/Action-Rclone)
