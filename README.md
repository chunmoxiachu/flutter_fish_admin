# 鱼来哒运营后台

Flutter Web 后台构建产物，使用 GitHub Pages 托管。

线上地址：

https://chunmoxiachu.github.io/flutter_fish_admin/

后台采用管理员手机号 + 短信验证码登录，管理接口与审计日志由 Supabase 提供。

## 更新部署

在 Flutter 源码仓库中执行：

```bash
flutter build web \
  -t lib/admin/main.dart \
  --release \
  --base-href=/flutter_fish_admin/ \
  --no-wasm-dry-run
```

然后将 `build/web` 内容同步到本仓库根目录并推送。
