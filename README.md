```powershell
Set-Location E:\dsh\academic\task\project-lung
@'
# Lung CXR screening service

Machine-learning powered chest X-ray screening service with Docker, GitHub Actions and MLOps.

Documentation is added in chapter 12 of the project guide.
'@ | Set-Content -Encoding utf8 README.md
```

三条约定：

> 2. 受保护分支 `dev` / `staging` / `main` 一律**不直接 push**，只接受 PR。
> 3. 每个 PR 必须等 `lint`、`test`、`docker` 三个检查全绿才能合并。
> 4. 合并方向只能是 `feature → dev → staging → main`。

> Repository skeleton created on 2026-10-19.
