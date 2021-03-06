---
title: API | 七牛云存储
---

# API

[**应用接入与认证授权**](/v3/api/auth/)

- [应用接入](/v3/api/auth/#app-access)
- [认证授权](/v3/api/auth/#app-auth)
    - [请求签名](/v3/api/auth/#req-signature)
        - [流程](/v3/api/auth/#workflow)
        - [示例](/v3/api/auth/#examples)
            - [PHP 数字签名示例程序](/v3/api/auth/#php-example)
            - [Ruby 数字签名示例程序](/v3/api/auth/#ruby-example)
    - [请求认证](/v3/api/auth/#req-auth)

[**云存储接口**](/v3/api/io/)

- [创建空间](/v3/api/io/#mkbucket)
- [上传文件](/v3/api/io/#upload)
    - [生成上传授权凭证](/v3/api/io/#upload-token)
        - [算法](/v3/api/io/#upload-token-algorithm)
        - [样例](/v3/api/io/#upload-token-examples)
    - [授权直传文件](/v3/api/io/#upload-file)
        - [API（multipart/form-data）](/v3/api/io/#upload-file-by-multipart)
        - [HTML表单形式直传](/v3/api/io/#upload-file-by-html-form)
    - [回调处理](/v3/api/io/#callback-after-uploaded)
        - [回调逻辑](/v3/api/io/#callback-logic)
        - [作为代理](/v3/api/io/#callback-as-proxy)
- [断点续上传](/v3/api/io/#resumable-upload)
    - [术语](/v3/api/io/#resumable-upload-keywords)
    - [工作模型](/v3/api/io/#resumable-upload-model)
    - [流程](/v3/api/io/#resumable-upload-workflow)
    - [API](/v3/api/io/#resumable-upload-api)
        - [授权](/v3/api/io/#resumable-upload-authorization)
        - [创建分割块（Block）并上传第一个数据块（Chunk）](/v3/api/io/#resumable-upload-mkblk)
        - [上传分割块（Block）中的数据块（Chunk）](/v3/api/io/#resumable-upload-bput)
        - [合并文件](/v3/api/io/#resumable-upload-mkfile)
    - [样例](/v3/api/io/#resumable-upload-examples)
- [下载文件](/v3/api/io/#download)
    - [公有资源下载](/v3/api/io/#public-download) 
    - [私有资源下载](/v3/api/io/#private-download)
    - [设置源文件(比如原图)保护](/v3/api/io/#set-protected)
        - [为指定的存储空间设置保护模式](/v3/api/io/#pub-access-mode)
        - [设置友好URL访问中的连接符](/v3/api/io/#pub-separator)
        - [设置URL友好的风格样式名](/v3/api/io/#pub-style)
        - [取消URL友好风格的样式名访问](/v3/api/io/#pub-unstyle)
    - [防盗链设置](/v3/api/io/#anti-theft-chain)
        - [设置防盗链模式](/v3/api/io/#uc-antiLeechMode)
        - [更新防盗链记录值](/v3/api/io/#uc-referAntiLeech)
    - [自定义 404 NotFound](/v3/api/io/#download-if-notfound)
    - [断点续下载](/v3/api/io/#download-by-range-bytes)
- [查看文件基本属性信息](/v3/api/io/#stat)
- [复制文件](/v3/api/io/#copy)
- [移动文件](/v3/api/io/#move)
- [删除指定文件](/v3/api/io/#delete)
- [删除所有文件（整个空间/Bucket）](/v3/api/io/#drop)
- [批量操作](/v3/api/io/#batch)
    - [批量获取文件基本属性信息](/v3/api/io/#batch-stat)
    - [批量复制文件](/v3/api/io/#batch-copy)
    - [批量移动文件](/v3/api/io/#batch-move)
    - [批量删除文件](/v3/api/io/#batch-delete)
- [清除指定空间缓存](/v3/api/io/#refresh-bucket)
- [列出所有空间（Buckets）](/v3/api/io/#list-all-buckets)

[**图像处理接口**](/v3/api/foimg/)

- [获取图片基本信息](/v3/api/foimg/#imageInfo)
- [获取图片EXIF信息](/v3/api/foimg/#imageExif)
- [生成指定规格的缩略图](/v3/api/foimg/#imageView)
- [高级图像处理接口（缩略、裁剪、旋转、转化）](/v3/api/foimg/#imageMogr)
- [高级图像处理接口（缩略、裁剪、旋转、转化）并持久化存储处理结果](/v3/api/foimg/#imageMogrAs)
- [图像水印接口](/v3/api/foimg/#watermark)

[**音频 / 视频处理接口**](/v3/api/avfop/)

- [音频转换](/v3/api/avfop/#audio-convert)
- [视频转换](/v3/api/avfop/#video-convert)
- [视频帧缩略图](/v3/api/avfop/#video-thumbnail)

[**理解常用术语**](/v3/api/words/)

- [Entry](/v3/api/words/#Entry)
- [EntryURI](/v3/api/words/#EntryURI)
- [EncodedEntryURI](/v3/api/words/#EncodedEntryURI)
- [URLSafeBase64Encode](/v3/api/words/#URLSafeBase64Encode)
- [MimeType](/v3/api/words/#MimeType)
- [EncodedMimeType](/v3/api/words/#EncodedMimeType)
- [CustomMeta](/v3/api/words/#CustomMeta)
- [EncodedCustomMeta](/v3/api/words/#EncodedCustomMeta)
- [FileCRC32Checksum](/v3/api/words/#FileCRC32Checksum)
- [VarExpression](/v3/api/words/#VarExpression)

[**错误码参照表**](/v3/api/code/)

- [认证错误码](/v3/api/code#acc)
