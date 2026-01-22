let qr;

function generateQR() {
  const url = document.getElementById('url').value.trim();
  const qrContainer = document.getElementById('qrcode');
  const loading = document.getElementById('loading');

  if (!url) return;

  qrContainer.innerHTML = '';
  loading.style.opacity = 1;

  setTimeout(() => {
    loading.style.opacity = 0;
    qr = new QRCode(qrContainer, {
      text: url,
      width: 220,
      height: 220,
      colorDark: '#00f5ff',
      colorLight: 'transparent',
      correctLevel: QRCode.CorrectLevel.H
    });
  }, 800); // 模擬計算動畫延遲
}
