# Waveshare ESP32-S3-AUDIO-Board

产品链接：https://www.waveshare.net/shop/ESP32-S3-AUDIO-Board.htm

## R76S 无屏变体

`esp32-s3-audio-board-r76s-headless` 用于未安装显示屏和摄像头的硬件：

- 不初始化 LCD、背光、SPI 和摄像头；
- 保留 ES8311 播放、ES7210 双麦、BOOT 按键和 RGB 灯；
- 通过 TCA9555 EXIO8 启用扬声器功放；
- 启用设备端 AEC，使用 codec 的播放参考通道；
- 默认从 `http://192.168.4.2:8080/xiaozhi/ota/` 获取 R76S WebSocket 配置。

构建：

```bash
python scripts/build.py waveshare/esp32-s3-audio-board \
  --name esp32-s3-audio-board-r76s-headless
```
