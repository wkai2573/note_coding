在瀏覽器按 F12 打開開發者工具，切換到 Console 分頁。
貼上並執行以下程式碼。
觀察 Console 輸出。

```javascript

// 取得 token
const token = localStorage.getItem('auth_token');

// 建立 WebSocket 連接
const socket = new WebSocket('wss://YOUR_SITE/api/core/graphql', 'graphql-transport-ws');

// 連接成功時觸發
socket.onopen = () => {
  console.log('✅ WebSocket 連接成功');
  // 發送 connection_init 訊息（依規範可帶 payload）
  socket.send(JSON.stringify({
    type: 'connection_init',
    payload: { headers: { Authorization: `Bearer ${token}` } }
  }));
};

// 接收訊息
socket.onmessage = (event) => {
  console.log('📩 收到訊息:', event.data);
};

// 錯誤
socket.onerror = (error) => {
  console.error('❌ WebSocket 錯誤:', error);
};

// 關閉
socket.onclose = (event) => {
  console.log('🔌 連接關閉:', event.code, event.reason);
};
(event) => {
  console.log('🔌 連接關閉:', event.code, event.reason);
}
VM240:9 ✅ WebSocket 連接成功
VM240:19 📩 收到訊息: {"payload":{"headers":{"Authorization":"Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE3OTEzNDU3ODksImlhdCI6MTc4ODc1Mzc4OSwidXNlcklEIjoiYmQxMzQ5YjktNmM1MC00OGYwLWFkM2QtYTZjYmE2N2IwNzNkIn0.Nq76KS8VTESWf-KF7oE3HolHPlTHfcnotbfjJdJy7zg"}},"type":"connection_ack"}

// 取得 token
const token = localStorage.getItem('auth_token');

// 建立 WebSocket 連接
const socket = new WebSocket('wss://kjrag-dev.rexyzdigital.com/api/graphql', 'graphql-transport-ws');

// 連接成功時觸發
socket.onopen = () => {
  console.log('✅ WebSocket 連接成功');
  // 發送 connection_init 訊息（依規範可帶 payload）
  socket.send(JSON.stringify({
    type: 'connection_init',
    payload: { headers: { Authorization: `Bearer ${token}` } }
  }));
};

// 接收訊息
socket.onmessage = (event) => {
  console.log('📩 收到訊息:', event.data);
};

// 錯誤
socket.onerror = (error) => {
  console.error('❌ WebSocket 錯誤:', error);
};

// 關閉
socket.onclose = (event) => {
  console.log('🔌 連接關閉:', event.code, event.reason);
};

```