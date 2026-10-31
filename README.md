# lilac_dcm 内核编译 (GitHub Actions)

用法：
1. 在 GitHub 新建一个**私有**空仓库（比如 lilac-kernel-ci），不要加 README。
2. 把本目录的 `.github/workflows/build-kernel.yml` 传上去（网页 Add file -> Upload files 即可，路径要一致）。
3. 进 Actions 页 -> build-lilac-dcm-kernel -> Run workflow。
4. 约 30-40 分钟后，在运行详情页底部下载 `kernel-output` artifact，里面有：
   - Image.gz-dtb
   - build.log
   - kernel.config

如果失败，把 build.log 发出来即可定位。