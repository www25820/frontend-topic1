# 前端专题1 · 优化后的示例页面

本仓库包含「专题1 前端前尘往事」课程中 5 个 HTML 示例页面的**修复优化版本**。

## 文件说明

| 文件 | 说明 | 主要修复 |
|---|---|---|
| `v-model.html` | Vue 3 双向绑定 | 本地 Vue 库不存在 → 改用 CDN；`lang="zh-CN"`；默认值；placeholder |
| `ajax-js原生.html` | 原生 JS AJAX | innerHTML 拼接未转义 → 增加 HTML 转义（防 XSS）；增加 8s 超时 |
| `ajax-jQuery.html` | jQuery AJAX | 同 XSS 转义；`$.ajax` 增加 `timeout`；文件名拼写修正 |
| `ajax-vue.html` | Vue 3 AJAX | 增加 AbortController 超时 + 请求竞态处理；抽 `isEmpty` 计算属性 |
| `ajax-js原生实现过程演示.html` | 交互式流程演示 | 统一接口地址；快捷键聚焦判断；子动画定时器统一清理 |

## 在线预览

- [Vue 双向绑定](v-model.html)
- [原生 JS AJAX](ajax-js原生.html)
- [jQuery AJAX](ajax-jQuery.html)
- [Vue 3 AJAX](ajax-vue.html)
- [AJAX 实现流程演示](ajax-js原生实现过程演示.html)

> 提示：页面通过 CDN 引入 Vue / jQuery 与免费的 JSONPlaceholder 测试接口，预览时需联网。
