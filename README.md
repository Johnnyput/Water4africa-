# Water4africa-
Building clean and good water for the features 
<div class="donation-container">
  <h2>Donate to Water4Africa</h2>
  <div class="wallet-options">
    <div class="wallet">
      <h3>Bitcoin (BTC)</h3>
      <p>Wallet Address: <span id="btc-address">bc1qvcamlt07ptyred7h7ll73ftkgnptd93wpceq7t</span></p>
      <button onclick="copyWalletAddress('btc-address')">Copy Wallet Address</button>
      <img src="btc-qr-code.png" alt="BTC QR Code">
    </div>
    <div class="wallet">
      <h3>Ethereum (ETH)</h3>
      <p>Wallet Address: <span id="eth-address">0x8854ba4cdc78501796405c2a33b99c2eb9c8490b</span></p>
      <button onclick="copyWalletAddress('eth-address')">Copy Wallet Address</button>
      <img src="eth-qr-code.png" alt="ETH QR Code">
    </div>
    <div class="wallet">
      <h3>USDT (Ethereum)</h3>
      <p>Wallet Address: <span id="usdt-eth-address">0x8854ba4cdc78501796405c2a33b99c2eb9c8490b</span></p>
      <button onclick="copyWalletAddress('usdt-eth-address')">Copy Wallet Address</button>
      <img src="usdt-eth-qr-code.png" alt="USDT (Ethereum) QR Code">
    </div>
    <!-- Add more wallet options as needed -->
  </div>
  <div class="transaction-tracker">
    <p>Total Donations: <span id="total-donations">...</span></p>
    <p>Number of Transactions: <span id="num-transactions">...</span></p>
  </div>
</div>

<script>
  function copyWalletAddress(elementId) {
    const walletAddress = document.getElementById(elementId).textContent;
    navigator.clipboard.writeText(walletAddress).then(() => {
      alert('Wallet address copied to clipboard!');
    });
  }
</script>
