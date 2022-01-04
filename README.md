# actions\_build\_recover, Custom Mods by Eliminater74

![](demo.jpg)

---

A Github Action to build Recovery

![](../../workflows/rec-building/badge.svg)

  
 

Due to the long compilation time, it is recommended to change the [`.github/workflows/actions_recovery.yml`](https://github.com/Eliminater74/actions_build_recovery/blob/master/.github/workflows/actions_recovery.yml)upload at the end `${{ secrets.GITHUB_TOKEN }}`to your own [Personal Access Token](https://github.com/settings/tokens)

To protect your Personal Access Token, put it in a warehouse [Settings](https://github.com/Eliminater74/actions_build_recovery/settings) in the [Secrets](https://github.com/Eliminater74/actions_build_recovery/settings/secrets) inside after use `${{ secrets.YOUR_TOKEN_NAME }}`to replace`${{ secrets.GITHUB_TOKEN }}`

For example, my secret name is work. Then use`${{ secrets.work }}`

## 配置

## **Configuration**

The configuration file is [config.json](https://github.com/Eliminater74/actions_build_recovery/blob/master/config.json)

| **name** | **type** | **describe** |
| --- | --- | --- |
| `twrp_url` | String | Recovery Manifest address |
| `twrp_branch` | String | Recovery Manifest branch |
| `git_username` | String | Your username with Git |
| `git_email` | String | Your Git mailbox (available on Github `Github ID+Github用户名@users.noreply.github.com`) |
| `use_own_dt` | Boolean | Indicate whether to use the personal device tree (this item is `true`effective for the following three items) |
| `dt_url` | String | Address of the device tree you use (format: `USER/REPO`) |
| `dt_branch` | String | Branch of the device tree you use |
| `dt_remote` | String | You use the repository of the device tree (as in `github/gitlab`) |
| `dt_path` | String | Indicate the local save location of the device tree (example `device/huawei/kiwi`) |
| `device_code` | String | The model code of the model you are about to compile |
| `fix_product` | Boolean | Indicates whether to fix the problem that the device cannot be found |
| `fix_branch` | String | Indicate the branch used to fix the above problem |
| `fix_misscom` | Boolean | Indicates whether to fix missing `device/qcom/common`issues |
| `fix_busybox` | Boolean | Indicates whether to fix missing `busybox`issues |

## **Start**

After Fork this warehouse, click on Star in the upper right corner to start

## **Compilation result**

Can be downloaded in [Release](https://github.com/Eliminater74/actions_build_recovery/releases)
