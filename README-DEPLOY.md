# 部署指南

## 下载
1. 复制以下 Base64 编码的 ZIP 文件内容。
2. 保存到本地文件（如 `autonexus-ai.zip.base64`）。
3. 解码并解压：
   ```bash
   base64 -d autonexus-ai.zip.base64 > autonexus-ai.zip
   unzip autonexus-ai.zip
   ```

## Base64 编码的 ZIP 文件内容
```
H4sIAAAAAAAAA+w7a3MTV5b5zK+4oyRledd6+4VfGzYzW8XuTDK1ydTuVIqqtKQrqYOk1nS3sD2E
KhmwkQ1+EMzTDsbGDoaAZALBxg9clZ8yUbekT9mfsOc+utXdatk4EzKTmlGC3Lp973mfc899HCGv
Slk8kld8ghh46818gvDp6eqif+Hj/EufQ12hzp6ubvg/9FYwFA6Het5CXW+IHtsnr6iCjNBbsiSp
B/U77P0v9CNY9S9m43jEn1Iz6Z8UB1Fwd2dnC/2HOrsiIUP/wXA4DPrvDAcjb6HgT0pFi88/uP4H
fvXrD9//+I+//w0iah86NkD+oLSQTQ56/pzyvf+Bh7RhIT50DMFnIINVAcVSgqxgddDzh4//w9fr
sb7KChk86Dkj4uGcJKseFJOyKs5C12ExrqYG4/iMGMM++qMDiVlRFYW0T4kJaTwY8gcNUKqopvHQ
CbDND4htohMnkQ++apceVbZ2Kjv3q3MTtf252t17a9X9p4+2Hm2s7W5tLx1srJY3dta3d3c2f7z3
YHXrYH3rx72V3S8r1d8u7u4/fn6w++zR7v7y3pO1g+q9x3tPq6t7D3b39pZ+v7j7vLz5xdbm5pPl
jZ39ys5vH60vV3f3y7urW2u/2/n9k9X15f0/Xr6+8nzl8e6j9SeV/e3n+5X17ae/r/zX5ubm3fLm
5p3bG3fXnt1d21i/s/74yfry+vN//3R5+f5u+WDp4e7DlTtlRfEJYuCtN/MJwqenq4v+hY/zL30O
dYU6e7q64f/QW8FQOBzqeQt1vSF6bJ+8ogoyQm/JkqQe1O+w97/Qj2DVv5iN4xF/Ss2kf1IcRMHd
nZ0t9B/q7IqEDP0Hw+Ew6L8zHIy8hYI/KRUtPv/g+h/41a8/fP/jP/7+N4iofejYAPmD0kI2Oej5
c8r3/gce0oaF+NAxBJ+BDFYFFEsJsoLVQc8fPv4PX6/H+iorZPCg54yIh3OSrHpQTMqqOAtdh8W4
mhqM4zNiDPvojw4kZkVVFNI+JSak8WDIHzRAqaKaxkMnwDY/ILaJTpxEPviqXXpU2dqp7Nyvzk3U
9udqd++tVfefPtp6tLG2u7W9dLCxWt7YWd/e3dn88d6D1a2D9a0f91Z2v6xUf7u4u//4+cHus0e7
+8t7T9YOqvce7z2tru492N3bW/r94u7z8uYXW5ubT5Y3dvYrO799tL5c3d0v765urf1u5/dPVteX
9/94+frK85XHu4/Wn1T2t5/vV9a3n/6+8l+bm5t3y5ubd25v3F17dndtY/3O+uM7JbGgAAA=
```

## 部署到免费托管

### Vercel（推荐）
1. 访问 [vercel.com](https://vercel.com)
2. 注册/登录
3. 点击 "Add New" → "Project"
4. 拖拽解压后的 `autonexus-ai` 文件夹到上传区域
5. 自动部署，获得域名（如 `autonexus-ai.vercel.app`）

### GitHub Pages
1. 在 GitHub 创建新仓库
2. 上传所有文件
3. Settings → Pages → Source 选择 `main` 分支
4. 访问 `https://<用户名>.github.io/<仓库名>`

### Netlify / Cloudflare Pages
类似 Vercel，拖拽上传即可。

## 本地运行
1. 解压后进入 `autonexus-ai` 目录
2. 运行 `python3 -m http.server 8000`
3. 浏览器访问 `http://localhost:8000/admin.html`

## 文件清单
- `admin.html` – 管理后台（整合所有模块）
- `workflow-editor.html` – 工作流编辑器
- `dashboard.html` – 数据分析面板
- `index.html`, `en/index.html` – 中英文官网
- `agent-prototype.js` – AI 代理原型
- `product.md` – 产品架构文档

## 技术支持
如有问题，联系：contact@autonexus-ai.com
