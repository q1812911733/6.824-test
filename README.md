<p align="center">
  <img alt="Chef Logo" src="https://avatars2.githubusercontent.com/u/24697112?v=3&s=200" height="150" />
  <h3 align="center">Chef</h3>
  <p align="center">Megvii通用的包管理工具，提升服务编排与部署效率</p>
</p>

---

## 设计目标

- 解决旧编排工具的痛点。
- 利用云原生理念，屏蔽掉底层multi-cloud不同的部署形式。
- 将版本管理、编排、部署关联并统一起来，便于在公司内推广使用。
- GitOps + client command + server，为开发运维提供高效的支持。

## 优势

- 版本管理更清晰，支持[semVer](https://semver.org/)方式过滤包，开发者可以部署不同形态的软件包（stable, release, latest...），系统发布版本时可以锁定各组件对应版本，保证部署的确定性。
- 强大的通用性适合各业务线使用
- recipe与combo两个层级使得无论从开发视角还是交付视角效率都会有显著的提升。
- 依赖管理完备而又灵活，提供可视化手段展示依赖关系
- 部署的确定性得以保证，避免同一个部署方案部署的系统不一致
- 模块的灵活解耦大幅提升了可扩展性，方便兼容其他OAM（e.g `kubevela`）及其他云平台
- 为动态算力分配，持续部署等提供方案支撑

## 通用性

- 支持多种包类型
  - helm chart
  - recipe
  - customized pkg （TODO）
- 支持多种渲染方式
  - go template
  - starlark（COMMING）
- 支持多种包存储平台
  - devops app-template-store
  - Local filesystem
- 支持多种部署平台
  - devops
  - k8s（基于helm chart）
  - mcd （TODO）
  
## 文档

https://chef.mcd.megvii-inc.com/doc/#/
