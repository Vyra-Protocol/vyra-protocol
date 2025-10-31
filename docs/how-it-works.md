# How Vyra Works

Request → **402** → Pay on Solana → Backend verifies → Retry with `x-vyra-paid:true` → **200 OK**.

The SDK automates client steps. Backend provides:
- /api/solana/blockhash
- /api/solana/send
- /api/verify
- protected resource endpoint returning 402 until paid
