# website-build-upload-oss
 把Git文档编译成静态HTML文件并上传到oss存储


# Usage

See [action.yml](action.yml)

用例:

```yaml
steps:
  - uses: Ant-OSS-Utility-Set/website-build-upload-oss@main
  - uses: manyuanrong/setup-ossutil@v2.0
    with:
      endpoint: "oss.aliyuncs.com"
      access_key: "your_key_id"
      access_secret: "your_key_secret"
      bucket: "your oss bucket"
      build_script_path:"Your script for building static HTML files，such as command :hugo "
```

参数

- **endpoint**：填写 Bucket 所在地域的域名信息，可参考访问域名和数据中心。
- **access_key**： oss的访问key。
- **access_secret**：oss的访问secret
- **bucket**：oss的bucket名称
- **build_script_path**：构建静态HTML的脚本路径


# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
