# Cloudflare-Express-Proxy
# 云速通道
> 基于 Cloudflare Worker 实现，提供高性能、强隐私保护的 Web 内容加速与代理服务。适用于突破地理限制、加速访问等场景。
> 
> A high-performance, privacy-focused web acceleration and proxy service based on Cloudflare Worker. Ideal for bypassing geo-restrictions and accelerating web access.

## 功能简介
本项目基于 Cloudflare Worker 实现，提供高性能、强隐私保护的 Web 内容加速与代理服务。适用于突破地理限制、加速访问等场景。

- **访问被墙或限速的国际网站**

- **作为个人隐私加速通道**

- **通过自定义域名实现专属加速入口**

## 使用教程

### 1. 部署到 Cloudflare Workers
1. 注册并登录 [Cloudflare](https://dash.cloudflare.com/)。
2. 新建 Worker 服务，将本项目 `worker.js` 代码粘贴到 Worker 编辑器。
3. 保存并部署。
4. 绑定自定义域名（可选）。

### 2. 使用方法
- 直接访问 Worker 根路径（如 `https://your-worker.workers.dev/`）进入主界面。
- 在输入框输入目标网址，点击"开始访问"即可加速跳转。
- 支持历史记录、自动进入、记住地址等便捷功能。
- 支持中英文界面切换。
- 代理访问时自动进行指纹、IP、时区、语言等多维度伪装，提升隐私与兼容性。

## 注意事项
- 本项目已实现高级指纹伪装（UA、IP、时区、语言、Canvas、WebRTC等），但部分极端检测站点仍可能识别代理行为。
- 支持自动混淆（见 `.github/workflows/obfuscate-worker.yml`），如需更高安全性可调整混淆参数。
- 仅支持现代浏览器，部分老旧浏览器或特殊UA可能兼容性较差。
- Cloudflare Worker有免费额度限制，大流量请关注官方计费政策。
- 请注意不要滥用该服务，确保只将它用于合法和合适的用途。

## 免责声明
- **责任限制**：作者不对脚本可能导致的任何安全问题、数据损失、服务中断、法律纠纷或其他损害负责。使用此脚本需自行承担风险。

- **不当使用**：使用者需了解，本脚本可能被用于非法活动或未经授权的访问。作者强烈反对和谴责任何不当使用脚本的行为，并鼓励合法合规的使用。

- **合法性**：请确保遵守所有适用的法律、法规和政策，包括但不限于互联网使用政策、隐私法规和知识产权法。确保您拥有对目标地址的合法权限。

- **自担风险**：使用此脚本需自行承担风险。作者和 Cloudflare 不对脚本的滥用、不当使用或导致的任何损害承担责任。

- **此免责声明针对非中国大陆地区用户，如在中国大陆地区使用，需遵守相关地区法律法规，且由使用者自行承担相应风险与责任。**

---

## 参考项目
- 本项目部分设计和实现思路参考自 [ymyuuu/Cloudflare-Workers-Proxy](https://github.com/ymyuuu/Cloudflare-Workers-Proxy)
- AI人工智能

