## AutoPackageScript
自动打包ipa，上传fir.im脚本
## Usage
将 `AutoPackageScript` 整个文件夹拖入到项目主目录

打开 `AutoPackageScript.sh` 文件修改自定义部分相关参数：`scheme_name` `is_workspace`  `is_uploadfir` `fir_token`

打开终端, `cd` 到 `AutoPackageScript` 文件夹，输入 `sh AutoPackageScript.sh` 命令，或者 执行 `sudo AutoPackageScript.sh脚本文件的路径`

如果是要上传到蒲公英托管平台，可将上传至fir.im平台的脚本代码进行修改，执行 `curl -F "file=@/tmp/example.ipa"  -F "uKey=xxx" -F "_api_key=xxx" https://qiniu-storage.pgyer.com/apiv1/app/upload` 请根据开发者自己的账号，将其中的 uKey 和 _api_key 的值替换为相应的值。 
具体API请参考 https://www.pgyer.com/doc/api#uploadApp
