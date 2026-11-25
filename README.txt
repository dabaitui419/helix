HELIX 双螺旋收益计算器 · 网站部署说明
=====================================

【网站包内容】
  index.html   ← 网站本体（单文件，无需服务器）
  README.txt   ← 本说明

【上线方式：Cloudflare Pages（推荐，免费、免 Git）】
1. 打开 https://dash.cloudflare.com/sign-up
   用邮箱 + 密码注册（免费），去邮箱点验证链接激活
2. 登录后：左侧菜单 Workers & Pages → Create → Pages → Upload assets（直接上传）
3. 项目名称填：helix-calc（或任意英文名）
4. 把本文件夹里的 index.html 拖进去（或上传 HELIX网站.zip）→ Deploy
5. 等 10~30 秒，得到网址：https://helix-calc.pages.dev
   （以后每次改版，重新上传一次即可更新）

【上线后测试清单】
  □ 顶部「⟳ 刷新实时数据」能拉到官方数字
  □ ② 右螺旋页 P 级名单能加载（230 人左右）
  □ 地址旁「复制」按钮能用（手机/电脑分别测）
  □ ① 收益测算输入能实时出结果
  □ ⑩ AiLGNS 观测台流动性池有数据
  □ ⑦⑧⑨ 合约查询/钱包资产/资金监控能查（走公共 RPC）

【注意】
  · 页面数据全部由浏览器实时拉取：官方 API（awakehelix.io）+ 观测站名单（jsdelivr）
  · 若个别 API 被跨域拦截，对应区块会提示「刷新失败」，不影响其他功能
  · 国内访问 pages.dev 偶有波动，如长期给国内用户看，可后续加自定义域名
