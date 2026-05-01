# 此刻在场 Demo 部署指南

## 本地预览

直接在浏览器打开 demo.html 即可（无需 npm）

## Vercel 部署

1. 将整个项目文件夹上传到 GitHub
2. 在 Vercel 导入该仓库
3. Framework Preset 选 Other
4. Output Directory 留空（根目录）
5. 点击 Deploy

## 素材文件夹结构

```
project/
├── demo.html
├── vercel.json
├── README.md
└── assets/
    ├── videos/
    │   ├── content_climax_female.mp4
    │   ├── content_buffer_female.mp4
    │   ├── digital_human_keep_moment.mp4
    │   ├── ad_drink_old.mp4
    │   ├── ad_drink_scene_01.mp4
    │   ├── ad_drink_scene_02.mp4
    │   └── ad_drink_scene_03.mp4
    └── images/
        ├── brand_momera_logo.png
        ├── brand_momera_slogan_card.png
        ├── digital_human_portrait.png
        ├── polaroid_result_fireworks.png
        └── scene_rebuild_triptych.png
```

注意：素材文件较大，建议用 Vercel 的 Large Files 功能或将视频托管到 CDN（如腾讯云 COS），更改 demo.html 中的视频 src。
