# 安裝
```shell
scoop install ffmpeg
```

### 網頁下載串流影片(.m3u8)

```shell
# 步驟:
# 1. 開啟F12
# 2. 關閉偵錯斷點 (不一定)
# 3. 重整
# 4. Netwrok 篩選 .m3u8
# 5. 找到index.m3u8
# 6. 右鍵 copy link address
# 7. 開啟終端輸入 "ffmpeg -i m3u8連結 檔名.mp4" enter
# 8. 到 %USERPROFILE% 找你的影片

# cmd執行以下命令，執行下載完影片會存在你的終端當前目錄

ffmpeg -i https://網址.m3u8 demo.mp4
```